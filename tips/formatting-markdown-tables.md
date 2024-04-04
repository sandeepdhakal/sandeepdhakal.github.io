---
title: Formatting markdown tables
date: 2024-03-28
tags: [vim,markdown,pandoc]
---

We can easily format a markdown table in vim using [pandoc](https://pandoc.org/MANUAL.html).
Starting with the below table

```markdown
| **Reference**                              | **Study area**    | **Status**        | **Scale**     | **Social component** |
| -------------------------------------------| ----------------- | ----------------- | ------------- | -------------------- |
| [Alves, R. G., Maia, R. F., et al. (2023)] | agriculture   | prototype     | local     | no |
| [Angin, P., Anisi, M. H., et al. (2020)] | agriculture   | architecture  | local     | no |
| [Bauer, P., Stevens, B., et al. (2021)] | earth systems | proposed    | supra-regional | yes, partial, proposed |
| [Buonocore, L., Yates, J., et al. (2022)] | environment | framework | local | no |
| [Calvin, K. and Bond-Lamberty, B. (2018)] | earth systems    | proposed | supra-regional | yes |
```

we can visually select the entire table and use pandoc to format the selection.
```vim
:'<,'>!pandoc -t commonmark_x
```

which generates the following formatted table:
```markdown
| **Reference**                              | **Study area** | **Status**   | **Scale**      | **Social component**   |
|--------------------------------------------|----------------|--------------|----------------|------------------------|
| [Alves, R. G., Maia, R. F., et al. (2023)] | agriculture    | prototype    | local          | no                     |
| [Angin, P., Anisi, M. H., et al. (2020)]   | agriculture    | architecture | local          | no                     |
| [Bauer, P., Stevens, B., et al. (2021)]    | earth systems  | proposed     | supra-regional | yes, partial, proposed |
| [Buonocore, L., Yates, J., et al. (2022)]  | environment    | framework    | local          | no                     |
| [Calvin, K. and Bond-Lamberty, B. (2018)]  | earth systems  | proposed     | supra-regional | yes                    |
```
