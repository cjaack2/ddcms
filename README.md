# 呆萌狮内容管理

## 简介
这是一个基于**JBoot**实现的内容管理手脚架。
目前实现了权限管理的部分，
项目讲持续更新，尽请期待。。。


## DDCMS 2.0 介绍

花了半个月时间,我推翻了1.0 重新重构代码,今天2月2号发布2.0

新特性:
* 新的后台ui更加精美
* 功能模块化
* 可以集群与非集群切换
* 支持代码生成
* 跟着实战书利用好代码生成,可以5分钟写一个功能基本CRUD
* 更多请自行发现 ^ . ^
.....

## DDCMS 2.0 项目实战书
配合这个项目写了一本教程书
https://www.kancloud.cn/zhoufeng/ddcms-doc


### 2018 先给项目画一个饼
![项目脑图](docs/imgs/nt.png)

## 近期更新
2018-2-2
- 更新ddcms2.0

2018-1-4
- 新增加首页前台静态模板
- 新增加首页置顶查询和文章查询
- 封装渲染模板工具类
- 为了实现动态主题功能,路径有所改动

2017-12-29
- 修复27号会话问题
- 兼容最新版jboot1.2.2
- 使用getBodyString() 1.2.2新特性方法
- 新增加用户中心前台静态模板
- 新增加用户设置前台静态模板
- 新增加用户文章前台静态模板
- 实现文章访问数量
- 更新数据库文件
- 新在增加前台用户发布文章
- 修复文章url为空时无法访问详情,为空取id查询文章
- 更新说明文档

2017-12-27
- 兼容jboot最新版1.2.1
- 实现文章管理部分,后台可以增删改查文章
- 实现前台文章列表展示
- 管理员权限在前台可以设置置顶或精华文章,并且在列表排序优先显示置顶文章
- 修复一些已知问题
注:目前比较简单,更多更新请关注ddcms

已知bug
- ~~会话在前台第一次能渲染数据,退出再次登录 报存在会话中的数据无法获取~~
- 目前后台的所有数据插入没有实现数据校验判断,先实现大功能在优化这些细节.


## 项目地址
- github ：https://github.com/zhoufengjob/ddcms
- 开源中国：https://gitee.com/zhoufengjob/ddcms


> 感谢jboot、layui、X-admin。本后端基于jboot架构，前端基于layui,X-admin。

##  声明
-  这个项目我站在巨人的肩膀上只用了10天时间完成权限管理v1.0.0
-  我没有webapp开发经验这里所有都是在这10天里面现学现用.在此之前没有接触过jfinal或enjoy.
-  我主要开发android程序,闲下来的时间学习web扩充知识点
-  如果项目中有不合理的地方请理解...
-  如果你有心可以提交发现的问题,大家一起学习...
-  我很喜欢jboot 原因是 上手简单
-  我在jboot官方1群,群号:601440615,欢迎来call

##  将来
我会继续跟新这个项目,利用学到的知识做一个完整的内容管理系统。


##   呆萌狮架构主要核心

核心依赖 | 名称及版本|版本号
---|---|---
后端框架 | Jboot |v1.2.2
后端工具|Hutool |v3.2.0
前端框架|layui |v2.x
前端依赖|xAdmin |v2.x
渲染引擎|enjoy |v3.3
sql 分离|enjoy |v3.3
核心驱动|jfinal |v3.3
权限框架|Shiro |v1.3.2


## 运行方法
1. 使用idea maven导入项目
2. 将docs下的sql导入数据库
3. 在项目根目录找到AppMain类执行Main方法

## 生成jar包方法
使用maven打包**窗口**运行程序:

```
clean package appassembler:assemble
```

使用maven打包**后台**运行程序:

```
clean package appassembler:generate-daemons
```




> 后台登录帐号:admin  
> 后台登录密码:admin




### 静态图展示
![后台主页](docs/imgs/login.jpg)
![登录](docs/imgs/index.jpg)
![弹窗图](docs/imgs/pop.jpg)
### 动态图
![登录图](docs/gits/login.gif)
![菜单展示](docs/gits/menu.gif)
![菜单展示2](docs/gits/menu2.gif)
![搜索展示](docs/gits/search.gif)
![响应式展示](docs/gits/xys.gif)

