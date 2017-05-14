---
layout:     post
title:      "一行代码完成所有请求，Retrofit2 + Rxjava2 封装记录"
subtitle:   " \"我也要来一个浮夸的标题\""
date:       2017-04-20 12Retrofit2+Rxjava2
author:     "Zlc"
header-img: "img/post-bg-2015.jpg"
tags:
    - Retrofit2+Rxjava2
---
# 一行代码完成所有请求，Retrofit2 + Rxjava2 封装记录

###  一  Retrofit2 基本使用流程

#### 1.1、创建Retrofit实例

```
Retrofit retrofit = new Retrofit.Builder()
        .baseUrl("http://localhost:4567/")
        .build();
```

创建Retrofit实例时需要通过`Retrofit.Builder`,并调用`baseUrl`方法设置URL。
**注：** Retrofit2 的baseUlr 必须以 **/（斜线）** 结束，不然会抛出一个`IllegalArgumentException`。



