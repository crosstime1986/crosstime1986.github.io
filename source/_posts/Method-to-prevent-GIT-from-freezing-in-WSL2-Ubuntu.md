---
title: WSL2  Ubuntu 中 GIT 不卡的方法
date: 2024-03-28 22:05:27
tags:
---
只需要中 .zshrc 添加这两行
```shell
git config --global --add oh-my-zsh.hide-status 1
git config --global --add oh-my-zsh.hide-dirty 1
```
