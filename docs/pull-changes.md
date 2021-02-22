# Pulling changes

<!-- ```shell
git pull git@github.com:vives-web-essentials-2019/exercises.git master
``` -->

## Setup

To pull the latest updates you will first need to add the original repo on which this one was based. This only needs to be done once for every cloned instance:

```shell
git remote add base git@github.com:databases-2021/databases-practical.git
```

`base` is the name of remote repo. Now you should see two remotes when issuing the command `git remote -v`. For example:

```text
base     git@github.com:databases-2021/databases-practical.git (fetch)
base     git@github.com:databases-2021/databases-practical.git (push)
origin  git@github.com:databases-2021/databases-practical-<username>.git (fetch)
origin  git@github.com:databases-2021/databases-practical-<username>.git (push)
```

## Instructions

Now every time you wish to pull updates you need to follow these steps:

1. First make sure that you have no local changes. This can be seen by executing `git status`. It should state `nothing to commit, working tree clean`. If not, you first need to add and commit the changes (see section [Commit Changes](./commit-changes.md)).
2. Now issue the following command to pull the latest changes

```shell
git pull base master
```

![Pulling Changes](./img/pull_changes.png)
