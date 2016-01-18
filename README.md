
## 入门

### 1 - 简介

提前预览一下本project完成时的功能和样子.

### 2 - Package

解释如何添加和使用包,同时也把项目里面需要使用的package提前都加进去了.

### 3 - 目录结构

单项目创建的目录结构.

### 4 - 布局

MainLayout和HomeLayout编写

### 5 - 路由

'/'路径的路由显示

### 6 - 数据Schema

详细讲解Schema的写法

### 7 - 添加数据

通过quickForm添加数据

### 8 - 权限与发布

先使用如下包, 然后在运行的chrome界面里面安CTRL-M就可以在web页面看相关信息了


### 9 - 字段和数组

定义数组形式的子段并通过autoform添加

### 10 - 公有和私有设置

通过settins.json文件添加private和public的setting, 其中private的仅在server可见,public的在client也可见

### 11 -  样式

通过styl格式添加了一些样式,在webstorm里面编辑styl有比较好的用户体验

另外，展示一些html输入的技巧,比如

```
  ul>li*3>a 
```

按tab以后可以生成如下内容

```html
  <ul>
    <li><a href=""></a></li>
    <li><a href=""></a></li>
    <li><a href=""></a></li>
  </ul>
```

### 12 - 建立菜单列表

通过templete添加列表

### 13 - 模板订阅



### 14 - 路由参数



### 15 - 单条目订阅

### 16 - 重定向

### 17 - 输入输出重定向

登录登出的重定向,用了下面这个package

```
gwendall:auth-client-callbacks
```
注意, 这些代码仅是client端的,如果没有做判断,会报错

```javascript
if( Meteor.isClient ) {
  Accounts.onLogin(function () {
    FlowRouter.go('recipe-book');
  });

  Accounts.onLogout(function () {
    FlowRouter.go('home');
  });
}
```

### 18 - 更新

### 19 - 过滤

通过style的设置巧妙的解决不同状态下显示不同button的问题

### 20 - 状态显示

通过另外一种方式设置不同状态下不同button的显示问题

### 21 - 购物车


### 22 - 表单更新

autosave是个好功能

### 23 - 删除

通过session切换编辑和显示状态, 不过切换一次,所有都同步显示

### 24 - ReactiveVars

通过ReactiveVar在Template级别单独控制每个的显示

### 25 - 总结

New Recipe的处理

