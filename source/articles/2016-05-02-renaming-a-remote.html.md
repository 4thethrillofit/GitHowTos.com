---
title: Renaming a remote
date: 2016-05-02 07:19 UTC
tags: remote
---

Use the `git remote rename` command to rename an existing remote.
READMORE
<br />
<br />

```shell
git remote -v
# View existing remotes
origin  https://github.com/OWNER/REPOSITORY.git (fetch)
origin  https://github.com/OWNER/REPOSITORY.git (push)

git remote rename origin destination
# Change remote name from 'origin' to 'destination'

git remote -v
# Verify remote's new name
destination  https://github.com/OWNER/REPOSITORY.git (fetch)
destination  https://github.com/OWNER/REPOSITORY.git (push)
```
