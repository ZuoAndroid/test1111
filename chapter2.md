---
layout: post
title: 在Deepin系统中安装Mysql数据库
categories: Deepin
description: Deepin安装MySQL
keywords: Deepin, Mysql
---
#在Deepin系统中安装Mysql数据库
其实在Deepin和Ubuntu上安装Mysql数据库很简单，只需要三条命令就可以搞定
## 安装mysql-server
```
sudo apt-get install mysql-server
```
【注意】：在此安装过程中会提示设置密码
## 安装mysql-client
```
sudo apt-get install mysql-client
```
## 安装libmysqlclient-dev
```
sudo apt-get install libmysqlclient-dev
```
## 安装完检查安装情况
安装完成之后，我们可以在终端中使用以下命令来检查是否安装成功：
```
sudo netstat -tap | grep mysql
```
通过上述命令检查之后，如果看到有mysql 的socket处于 listen 状态则表示安装成功。
## 登录mysql
```
mysql -u 用户名 -p 密码
```
