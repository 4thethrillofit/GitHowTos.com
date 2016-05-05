---
title: Changing a remote’s url
date: 2016-05-03 16:46 UTC
tags: remote
---

The `git remote set-url` command changes an existing remote repository URL.
READMORE
<br /><br />

```bash
# List existing remotes to get the name of the remote you want to change
$ git remote -v
origin  git@github.com:USERNAME/REPOSITORY.git (fetch)
origin  git@github.com:USERNAME/REPOSITORY.git (push)

# Change your remote's URL
$ git remote set-url origin git@github.com:USERNAME/NEW_REPOSITORY.git

# Verify that the remote URL has changed.
$ git remote -v
origin  https://github.com/USERNAME/NEW_REPOSITORY.git (fetch)
origin  https://github.com/USERNAME/NEW_REPOSITORY.git (push)
```

<br /><br />
_[source](https://help.github.com/articles/changing-a-remote-s-url/)_

