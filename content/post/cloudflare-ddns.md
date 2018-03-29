---
title: "使用Cloudflare实现DDNS"
date: 2018-03-29T16:49:01+08:00
draft: false
tags: ["php", "DDNS", "Cloudflare"]
---
很久之前，我写过一个用`Dnspod`实现动态ip解析的php脚本(想了解的可以看看[这里](https://github.com/shaojjjin/DNSPOD-DDNS)，不过当时的代码写得很烂哈哈)。不过随着这次将博客托管到`GitHub Pages`，为了启用https，我也不得不将域名的DNS解析服务转移到`Cloudflare`上来，所以之前实现的在`Dnspod`动态域名脚本也不能用了。

## 开始之前的准备

Cloudflare为开发者们提供了API，具体的API可以看看他们的[手册](https://api.cloudflare.com/)。

### 获取Cloudflare的相关信息

1. 登录账号
![获取邮箱](https://dn-imzeon.qbox.me/blog/180329/BH98339BJ1.png?imageslim)
其实就是你登录的邮箱，不确定的话可以打开 [https://www.cloudflare.com/a/profile](https://www.cloudflare.com/a/profile) 第一栏就是了。
2. API Key
![获取api_key](https://dn-imzeon.qbox.me/blog/180329/K8609k1ALj.png?imageslim)
在同一个页面，找到`API Key`这一栏，点击`view API Key`，输入自己的密码就能看到自己的API Key。
3. Zone id
![获取Zone_id](https://dn-imzeon.qbox.me/blog/180329/h1hd73jL9b.png?imageslim)
这个位于 “[https://www.cloudflare.com/a/overview](https://www.cloudflare.com/a/overview)” 的第二块区域 “Domain Summary” 的右侧。

### 获取脚本

> 未完待续。