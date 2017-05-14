---
layout:     post
title:      "Github Page 搭建指南（基础版）"
subtitle:   " \"Hello World, Hello Blog\""
date:       2017-05-06 12:00:00
author:     "Zlc"
header-img: "img/post-bg-2015.jpg"
tags:
    - 记录
---

# Github Page 搭建指南（基础版）

>  Github Page 是Github提供的开发者托管静态网页的一款产品，我们可以用来搭建自己或者项目的主页。
>
>  用户可以通过自己的github用户名直接访问托管的主页。

## 创建 Page仓库

首先，你必须在Github上创建Repository,使用 username.github.io 作为你的仓库名称。值得注意的是，此处的username必须与你的Github账户名一致。同时次仓库作为Github page仓库具有唯一性。

## 克隆仓库到本地编辑

Github上的Page仅用于网页托管以及访问入口。网页的具体内容任然需要我们自己进行编辑。

1. 使用` git clone https://github.com/username/username.github.io `命令clone你的仓库到本地
2. 执行` cd username.github.io ` , ` echo "Hello World">index.html`  在本地分支创建index.html主页

## 提交网页到仓库

在编辑完本地网页内容后，使用git提交相关修改到Github仓库。执行以下命令：

``` 
~ $ git add --all
~ $ git commit -m "Initial commit"
~ $ git push -u origin master
```


## 从浏览器访问

此时一个简单的网页就已经完成托管，在浏览器输入 http://username.github.io 就可以访问刚刚提交的index.html页面了。

## 后续：使用模板完善主页 

Github默认使用Jekyll作为主页模板，在官网上有许多模板可供选择，同时网上也能搜寻到许多用户开源的个人主页，后者相对功能完善，界面美观，使用起来也会非常方便。

作为一篇基础教程，简单的介绍就到这里了，后续有兴趣的可以自行百度~。





