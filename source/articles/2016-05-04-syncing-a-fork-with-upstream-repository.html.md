---
title: Syncing a fork with upstream repository
date: 2016-05-04 20:56 UTC
tags: remote, fork, open source
---

Sync your fork of a repository to keep it up-to-date with the upstream (the original) repository.
READMORE
<br /><br />

```bash
# Make sure the origin remote points to your fork
$ git remote -v
origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)

# Add the original repo as the upstream remote
$ git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git

# Verify you added the upstream remote successfully
$ git remote -v
origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (fetch)
upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (push)

# Get the latest updates from the original repo
$ git fetch upstream
remote: Counting objects: 75, done.
remote: Compressing objects: 100% (53/53), done.
remote: Total 62 (delta 27), reused 44 (delta 9)
Unpacking objects: 100% (62/62), done.
From https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY
 * [new branch]      master     -> upstream/master

# Check out your fork's local master branch.
$ git checkout master
Switched to branch 'master'

# Merge the changes from upstream/master into your local master branch.
# This brings your fork's master branch into sync with the upstream repository,
# without losing your local changes.
$ git merge upstream/master
Updating a422352..5fdff0f
Fast-forward
 README                    |    9 -------
 README.md                 |    7 ++++++
 2 files changed, 7 insertions(+), 9 deletions(-)
 delete mode 100644 README
 create mode 100644 README.md
```

<br /><br />
_[source](https://help.github.com/articles/syncing-a-fork/)_

