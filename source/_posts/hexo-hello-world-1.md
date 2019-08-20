---
title: Hexo搭建属于自己的博客(一) Hexo安装
date: 2019-07-08 13:31:41
description: Hexo新手教程，使用Hexo快速且高效的搭建博客。本文包含了hexo简介、并对hexo、hexo-cli安装进行了详细讲解。呵呵大王的博客--积累与分享。
keywords: Hexo安装、heco-cli、hexo教程
category: Hexo
tags: Hexo
lede: Hexo是一个快速、简洁且高效的静态博客框架，我们一起开安装使用Hexo。
thumbnail: /post_img/Hexo.jpg
---
## Hexo简介
**Hexo**是一个快速、简洁且高效的静态博客框架。Hexo 使用**Markdown**(或其他渲染引擎）解析文章，在几秒内，即可利用丰富多彩的主题生成静态网页。
## 为什么使用Hexo
**Hexo**是基于nodejs的静态博客框架。在动态网页大行其道的时代，为什么我们还要使用静态博客呢？本人是基于以下的原因选择了静态博客。
* 更加易于SEO。
* 前端社区越来越活跃，许多以前只能使用后端处理的业务也可以在前端方便的实现。
* 喜欢使用**Markdown**。
* 最最主要的是**成本低**，自己在[阿里云](https://promotion.aliyun.com/ntms/yunparter/invite.html?userCode=a00le4xj)搞一台最低配的**ECS**（一年600）或**云虚机**（一年200+）就可以搞定。什么？这也嫌贵？没关系GitHub有Hexo的免费托管服务，一毛钱都不用。

## Hexo安装
进入正题，开始安装Hexo

### Hexo的依赖
Hexo依赖于**nodejs**和**git**。
可以通过一下方法检验是有已经安装了**nodejs**和**git**
``` bash
# nodejs check
$ node --version
v10.15.0  # nodejs is installed

# git check
$ git --version
git version 2.15.1.windows.2  # git is installed
```
如果你的机器上已经安装好了,恭喜你可以跳过一下的依赖安装步骤

#### nodejs 安装
去Nodejs[官网](https://nodejs.org)下载安装
#### git 安装
* Windows：下载并安装 **git**[官网](https://git-scm.com/)或[国内镜像站](https://npm.taobao.org/mirrors/git-for-windows/).
* Mac：
``` bash
brew install git
```
* Linux (Ubuntu, Debian)：
``` bash
sudo apt-get install git-core
```
* Linux (Fedora, Red Hat, CentOS)：
``` bash
sudo yum install git-core
```
### Hexo-cli安装
安装好了git和nodejs后就可以通过**npm**安装**hexo-cli**了
``` Bash
$ npm install -g hexo-cli
```
但是，由于周所周知的原因。强烈建议使用**yarn**进行安装
``` Bash
$ yarn global add hexo-cli
```

安装完成使用如下命令检查
``` bash
$ hexo version
hexo: 3.9.0
hexo-cli: 2.0.0
os: Windows_NT 10.0.17134 win32 x64
http_parser: 2.8.0
node: 10.15.0
v8: 6.8.275.32-node.45
uv: 1.23.2
zlib: 1.2.11
ares: 1.15.0
modules: 64
nghttp2: 1.34.0
napi: 3
openssl: 1.1.0j
icu: 62.1
unicode: 11.0
cldr: 33.1
tz: 2018e
```
恭喜你可以开始使用Hexo写博客了。