---
title: 开发环境加速
tags: productivity
date: 2020-10-05 04:47:48
---


开发环境有很多工具，默认配置依赖国外的数据源，在国内使用，安装和更新都很不方便，替换成国内的数据源提速效果显著，使用感极佳，汇总下平常使用到的各个数据源配置，当做备忘。

### homebrew

[Mac安装Homebrew并更换国内镜像源](https://www.cnblogs.com/StivenYang/p/12546605.html)

### python pip

在`~/.pip/pip.conf`文件（没有则新建）中配置如下内容：

```shell
$ cat .pip/pip.conf
[global]
index-url = https://mirrors.aliyun.com/pypi/simple/
[install]
trusted-host = mirrors.aliyun.com
```

### node npm

```shell
# 设置国内源
$ npm config set registry https://registry.npm.taobao.org
# 查看源配置
$ npm config get registry
https://registry.npm.taobao.org/
```

### ruby gem

详细信息见官方教程：[RubyGems China](https://gems.ruby-china.com/)

```shell
$ gem source -l
*** CURRENT SOURCES ***

https://rubygems.org/

# 添加国内源
$ gem sources --add https://gems.ruby-china.com
https://gems.ruby-china.com added to sources

$ gem source -l
*** CURRENT SOURCES ***

https://rubygems.org/
https://gems.ruby-china.com

# 删除国外源
$ gem source -r https://rubygems.org/
https://rubygems.org/ removed from sources
```