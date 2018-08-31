---
layout: post
title: Linux操作命令
category: tech
tag: [linux]
---

Linux有些命令经常不用就会忘记，现在整理一下自己常用的，以后想到了再补充。


----------
## 目录处理

### 1、ls：列出目录
 
 - ls -a：全部的文件，连同隐藏的文档一起列出来；
 - ls -d：仅列出目录本身，而不是列出目录内的文件数据；
 - ls -l：长数据串列出，包含文件的属性与权限等等数据；

### 2、cd：切换目录
 
 - cd ..：回到目前的上一级目录；
 - cd ~：回到自己自己的家目录；
 - cd ./cosydays/：使用相对路径切换到cosydays目录；
 - cd /root/cosydays/：使用绝对路径切换到cosydays目录；

### 3、pwd：显示当前的目录

 - pwd -p：显示出确实的路径，而不是使用连结路径；

### 4、mkdir：创建一个新的目录

 - mkdir cosydays：创建一个名为cosydays的目录；

### 5、rmdir：删除一个空的目录

 - rmdir -p：连同上一级【空的】目录一起删除
 - rmdir cosydays：删除cosydays目录

### 6、cp：复制文件或目录

 - 

### 7、rm：移除文件或目录

