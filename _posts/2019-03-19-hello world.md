---
layout:     post
title:      Hello world
subtitle:    "\"Hello World, Hello Blog\""
date:       2019-03-19
author:     lisbeth
header-img: img/post-bg-hello.jpg
catalog: true
tags:
    - 生活
---

> “Hello !”


## 前言

我 的 Blog 就这么开通了。

本来打算在年前完成 Blog 的搭建，不曾料想踩了很多坑。。。

[跳过废话，直接看技术实现 ](#build) 

2019 年，我的 Blog 总算是搭建好了。



一直想搭建一个个人博客，由于种种原因一直没有弄。我觉得作为一名程序媛，怎么能能没有一个自己的博客呢？在一次偶然间发现github pages 搭建个人博客比较简单，于是就开始倒腾倒腾自己的Blog，于是乎就开始了撸起袖子干了。

<p id = "build"></p>
---

## 正文

接下来说说搭建这个博客的技术细节。  

正好之前就有关注过 [GitHub Pages](https://pages.github.com/) + [Jekyll](http://jekyllrb.com/) 快速 Building Blog 的技术方案，非常轻松时尚。

其优点非常明显：

* **Markdown** 带来的优雅写作体验
* 非常熟悉的 Git workflow ，**Git Commit 即 Blog Post**
* 利用 GitHub Pages 的域名和免费无限空间，不用自己折腾主机
	* 如果需要自定义域名，也只需要简单改改 DNS 加个 CNAME 就好了 
* Jekyll 的自定制非常容易，基本就是个模版引擎



---


主题我直接 Downlosd 了 [Hux的博客主题](https://huangxuan.me/) 的进行修改，简单粗暴，不过遇到了很多坑😂，好在都填完了。。。

本地调试环境需要 `gem install jekyll`，结果 rubygem 的源居然被墙了，~~后来手动改成了我大淘宝的镜像源才成功~~，淘宝的源已经[停止维护](https://gems.ruby-china.org/)，换成了OSChina的源 `https://gems.ruby-china.org/`。


## 后记

最后，感谢 Hux 提供的的 [Blog 主题](https://github.com/Huxpro/huxpro.github.io)

如果你恰好逛到了这里，希望你也能喜欢这个博客主题，感兴趣的话可以自己动手搭建一个。

—— lisbeth 后记于 2019.3


