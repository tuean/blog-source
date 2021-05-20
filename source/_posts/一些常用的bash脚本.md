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

### 查看项目占用内存
ps aux | grep *.jar | grep -v grep | awk '{print $11 "\t" $6/1024"MB" }'

### 端口使用情况
ss -nplt

### 替换文件信息
sed -i s/{old}/{new}/g `grep {old} -rl ./`

