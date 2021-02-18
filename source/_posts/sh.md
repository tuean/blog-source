---
title: sh
date: 2020-12-02 17:15:54
tags:
    - shell
cover: https://i.loli.net/2021/02/18/o7jSzVZ4n9RBl5I.jpg
---


### 查询大文件
find . -type f -size +800M

### 大文件路径
find . -type f -size +800M  -print0 | xargs -0 ls -l 

### 大文件详细大小
find . -type f -size +800M  -print0 | xargs -0 du -h 

### 文件大小排序
find . -type f -size +800M  -print0 | xargs -0 du -h | sort -nr

