---
title: Renaming a remote
date: 2016-05-02 07:19 UTC
tags: remote
---

Use the `git remote rename` command to rename an existing remote.
READMORE
<br />
<br />

```bash
# View existing remotes
$ git remote -v
origin  https://github.com/OWNER/REPOSITORY.git (fetch)
origin  https://github.com/OWNER/REPOSITORY.git (push)

# Change remote name from 'origin' to 'destination'
$ git remote rename origin destination

# Verify remote's new name
$ git remote -v
destination  https://github.com/OWNER/REPOSITORY.git (fetch)
destination  https://github.com/OWNER/REPOSITORY.git (push)
```

<br />
<br />
_[Read more](https://help.github.com/articles/renaming-a-remote/)_

