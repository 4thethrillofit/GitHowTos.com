---
title: Removing a remote
date: 2016-05-03 16:54 UTC
tags: remote
---

Use the `git remote rm` command to remove a remote URL from your repository.
READMORE
<br /><br />


```bash
# View current remotes
$ git remote -v
origin  https://github.com/OWNER/REPOSITORY.git (fetch)
origin  https://github.com/OWNER/REPOSITORY.git (push)
destination  https://github.com/FORKER/REPOSITORY.git (fetch)
destination  https://github.com/FORKER/REPOSITORY.git (push)

# Remove remote
$ git remote rm destination

# Verify it's gone
$ git remote -v
origin  https://github.com/OWNER/REPOSITORY.git (fetch)
origin  https://github.com/OWNER/REPOSITORY.git (push)
```



<br /><br />
_[source](https://git-scm.com/book/en/v2/Git-Basics-Working-with-Remotes)_

