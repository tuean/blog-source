---
title: git
date: 2019-09-29 16:52:02
tags: 
    - git
comments: true
cover: https://i.loli.net/2019/10/23/NtCopZqmeBSKOl1.jpg
description: some git commands
---

#### git相关命令

* 复制仓库
```bash
git clone --bare git://xxx.xx.xx.xx/git_repo/old_project_name.git
cd old_project_name.git
git push --mirror new_project.git
```

