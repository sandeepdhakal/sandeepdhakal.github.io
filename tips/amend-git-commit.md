---
title: Amend last git commit
date: 2024-04-18
tags: [git]
---

If we forget to include some file(s) with a git commit, or want to change the commit message, the `git commit --amend` is a convenient method. 

> [!warning]
> It should be noted that using `amend` will replace the last commit with the new commit, and the previous commit will no longer be on the current branch.

## Changing the commit message
When nothing else has been staged after the last commit,

```bash
git commit --amend -m 'updated commit message'
```

will simply let you change the last commit message.

## Changing commited files
If we forget to commit a file, we can do the following:

```bash
# add files
git add file1.py file2.py
git commit -m 'fixed an error...'

# when you realise you didn't include another file
git add file3.py
git commit --amend --no-edit
```

The `--no-edit` option lets you skip specifying a new commit message.



