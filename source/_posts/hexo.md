---
title: hexo配合github搭建博客
date: 2019-10-09 16:39:54
tags: 
    - hexo
    - github 
cover: http://pyjw54h3s.bkt.clouddn.com/103840-1542249520645d.jpg
comments: true
description: steps of building this blog 
---

### hexo + github pages 搭建博客

#### 软件安装
1. nodejs (hexo依赖nodejs， 已安装可跳过)
    * windows/mac 进入[node官方网址](https://nodejs.org/en/)下载最新版并安装
    * mac环境下可通过包管理器安装
        1. 安装homebrew[官网](https://brew.sh/) 或者通过以下命令
            ```bash
            /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
            ```
        2. 通过homebrew安装node
            ```bash
            brew install -g node
            ```
        3. 每次执行homebrew后都会先执行update 目前由于各种原因耗时很大，可通过以下命令关闭
            ```bash
            export HOMEBREW_NO_AUTO_UPDATE=true
            ```
     * 验证是否安装完成   
        ```bash
        node -v
        ```
        显示版本号即可

2. git (已安装可跳过)
    * windows下 [官网](https://git-scm.com/download/win)  
    * mac下 
        安装
        ```bash
        homebrew install git
        ```
        校验
        ```bash
        git --version
        ```
        显示版本号即可

3. 安装hexo
    1. 选择一空文件夹 例如 **blog** 
    2. 命令行进入上述文件夹
    3. 输入以下命令
        ```bash
        npm i -g hexo
        ```
    4. 