---
title: 如何批量删除所有git tag 和 branch
date: 2024-03-28 21:56:04
tags:
---

远程

```
git tag -l | xargs -n 1 git push --delete origin
```
本地
```
qi
```
远程分支：
```
git branch -a | grep "keyi" | sed 's/remotes\/origin\///g' | xargs git push origin --delete
```
本地分支
```
git branch |grep 'branchName' |xargs git branch -D
```
