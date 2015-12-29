---
layout: post
category : jekyll
title: "在Windows系统配置Jekyll"
tags : [jekyll]
---
{% include JB/setup %}

[Jekyll](http://jekyll.bootcss.com/) 是一个简单的网站静态页面生成工具。由于是用Ruby语音编写的，所以在Windows系统上配置起来还是稍微有点繁琐的。具体过程如下：


1. 安装Ruby：在Windows系统上当然使用rubyinstaller了， [下载](http://rubyinstaller.org/downloads/) 
2. 安装Ruby DevKit： [下载](http://rubyinstaller.org/downloads/)
3. 安装Jekyll
4. 安装Python
5. 安装Pygments


### 安装Ruby： ###

从rubyinstaller下载安装包并安装到某个磁盘中，比如：E:\Ruby192

![](/img/201509/1.png)

在安装界面把所有的选项都勾选上；

![](/img/201509/2.png)

打开一个命令提示行并输入以下命令来检测 Ruby 是否成功安装。

    ruby -v

### 安装Devkit ###

把下载的DevKit解压到某个目录，比如 E:\devkit , 在该目录中运行如下命令：

    ruby dk.rb init

来生成一个config.xml配置文件

    ruby dk.rb install

### 安装Jekyll ###

1、确保gem安装

    gem -v

输出实例

    2.4.8

开始安装jekyll

    gem install jekyll

### 安装 Python ###

[点击下载](http://www.python.org/download/)

下载合适的 Python windows 安装包安装

添加安装路径 (如： C:\Python27) 至 PATH。

检验 Python 安装是否成功

    python –V

输出示例：

    Python 2.7.6

## Next Steps

Please take a look at [{{ site.categories.api.first.title }}]({{ BASE_PATH }}{{ site.categories.api.first.url }})
or jump right into [Usage]({{ BASE_PATH }}{{ site.categories.usage.first.url }}) if you'd like.