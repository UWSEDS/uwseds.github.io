---
layout: page
title: Homework 1 Submission
---

# Homework 1 Submission

This guide will walk you through submitting homework 1 after you've finished developing your notebook. They assume you've a workspace directory setup with the following files:

````
> ls
homework1.ipynb
data/*
````

## 1: Clone Repo

Visit the github classroom to establish/access your personal homework repository: https://classroom.github.com/a/yiSZgFof 

From the repository page use the provided clone url to clone the remote repository into your workspace. For example:

````
> git clone https://github.com/UWSEDS-aut17/hw1-asford
> ls
data
homework1.ipynb
hw1-asford
````

## 2: Move homework into repository clone and commit

Move your homework submission into the repository folder and commit it to the repo.

````
> mv homework1.ipynb data hw1-asford
> cd hw1-asford
> ls
LICENSE
README.md
data
homework1.ipynb
> git status
On branch master
Your branch is up-to-date with 'origin/master'.
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	data/
	homework1.ipynb

nothing added to commit but untracked files present (use "git add" to track)
> git add .
> git commit
...
[master b4b3b65] Homework submission.
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 data/1
 create mode 100644 homework1.ipynb
````

## 3: Push homework to remote

Finally, push your homework submission to github for submission:

````
> git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)
nothing to commit, working tree clean
> git log --graph --oneline --decorate
* b4b3b65 (HEAD -> master) Homework submission.
* fb67da8 (origin/master, origin/HEAD) Update homework description for Autumn 2017.
* c55f61a added assingment text from google doc with updates for GitHub classroom
* 1e407c3 Initial commit
> git push origin
Counting objects: 4, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 422 bytes | 0 bytes/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To https://github.com/UWSEDS-aut17/hw1-asford
   fb67da8..b4b3b65  master -> master
> git log --graph --oneline --decorate
* b4b3b65 (HEAD -> master, origin/master, origin/HEAD) Homework submission.
* fb67da8 Update homework description for Autumn 2017.
* c55f61a added assingment text from google doc with updates for GitHub classroom
* 1e407c3 Initial commit
````
