---
title: Nodejs配置
banner_img: 
index_img: 
date: 2020-04-03 13:07:34
categories: 
tags: 
---

## Nodejs下载

[https://nodejs.org/download/release/](https://nodejs.org/download/release/)](https://nodejs.org/download/release/)

## 查询版本

```bash
node -v
npm -v
```

## 配置缓存路径

``````bash
npm config set prefix "D:\node_global"
npm config set cache "D:\node_cache"
//查询
npm config get cache
npm config get prefix

``````

## 配置源

```bash
//华为云镜像源
npm config set registry https://mirrors.huaweicloud.com/repository/npm/
//查询
npm config get registry
```

## 配置代理

```bash
npm config set proxy http://127.0.0.1:1080
npm config set https-proxy http://127.0.0.1:1081
//查询
npm config get proxy
npm config get https-proxy
```

## 查看npm配置信息

```bash
npm config list
```

