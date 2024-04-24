---
title: Using mamba solver with conda without installing mamba
short-title: Using mamba solver with conda
date: 2024-04-24
tags: [conda,mamba,python]
---

Installing packages with [anaconda/conda](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html) can be a slow and painful process, partly due to its default solver.
[Mamba](https://mamba.readthedocs.io/en/latest/index.html) solves this problem but it needs to be installed separately.
However installing `mamba` is not always possible, particularly in HPC environments where you don't have the requisite rights.

The `conda-libmamba-solver` package provides an elegant solution by allowing us to use the `libmamba` solver that is used by `mamba` directly in `conda`.

## Installation
The official [documentation](https://conda.github.io/conda-libmamba-solver/user-guide/) suggests that `conda-libmamba-solver` be installed on the `base` environment.
But in my case, I didn't have the rights to update the `base` environment. Therefore I ended up installing it on the environment where I'll be using this solver.

```bash
(ipm) ~> conda install conda-libmamba-solver
```

Once installed, you can now specify `libmamba` as the solver when installing packages. While the official docs don't mention this, but I also had to specify the `conda-forge` channel.
```bash
(ipm) ~> conda install geopandas --solver=libmamba --channel=conda-forge
```

## Setting as default
To enable the above settings permanently, you can add them to the `.condarc` file as follows:
```bash
(ipm) ~> conda config --set solver libmamba
(ipm) ~> conda config --add channels conda-forge
```

Now you should be able to install packages using `libmamba` from the `conda-forge` channel by default.
```bash
(ipm) ~> conda install sortedcontainers
```
