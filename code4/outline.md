# 大纲-day02

## session和cookie分析
- http协议是无状态的
- 但是实际情况我们需要维护客户端和服务器之间的状态
- 可以通过cookie和session解决这个问题

### cookie基本操作
- 获取cookie
- 设置cookie
- cookie分类
    + 会话cookie
    + 持久cookie
- cookie常用属性
    + expires 有效期
    + path cookie路径
- 封装cookie操作方式
    + 设置cookie
    + 获取cookie
- 使用jQuery插件操作cookie
    + 获取所有cookie
    + 获取指定cookie
    + 设置cookie
    + 删除cookie

### session操作
- session是服务器端技术
- session在开启的时候会生成一个唯一编号PHPSESSID
- session里面可以存储数据（这些数据与PHPSESSID相关联）

### cookie与session的关系
- session可以借助cookie
- 但是cookie可以被浏览器禁用
- 可以通过别的办法解决：URL重写

## 模块化开发概念
- 非模块化开发缺点
    + 命名冲突(EXTJS YUI EXJ.panel.abc())
    + 文件依赖
- 模板规范
    + 浏览器端模块化
        * AMD --- Require.js
        * CMD --- Sea.js
    + 服务器端的模块化
        * CommonJS --- Node.js

## requirejs基本使用

## 模块定义与加载

## git初始化仓库

## 完善登录功能

## 模块化重构登录功能






