
# [Intermediate Meteor Introduction](https://www.youtube.com/watch?v=BI8IslJHSag&list=PLLnpHn493BHFYZUSK62aVycgcAouqBt7V)

## 1 - Project Introduction

提前预览一下本project完成时的功能和样子.

## 2 - Package

解释如何添加和使用包,同时也把项目里面需要使用的package提前都加进去了.

## 3 - Project Structure

单项目创建的目录结构.

## 4 - Basic Layout

MainLayout和HomeLayout编写

## 5 - Basic Routing with Layout in Meteor

'/'路径的路由显示

## 6 - Defining A Schema in Meteor

详细讲解Schema的写法

## 7 - Easy Forms with AutoForm in 

通过quickForm添加数据

## 8 - Insert Permissions, Publishing & Meteor Toys

先使用如下包, 然后在运行的chrome界面里面安CTRL-M就可以在web页面看相关信息了

```
meteortoys:allthings
```

## 9 - Sub-documents & Array Fields

定义数组形式的子段并通过autoform添加

## 10 - Private & Public Settings and Google Analytics

通过settins.json文件添加private和public的setting, 其中private的仅在server可见,public的在client也可见

## 11 - Create Partials and Adding Styles

通过styl格式添加了一些样式,在webstorm里面编辑styl有比较好的用户体验

另外,视频中也展示了一些html输入的技巧,比如

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

## 12 - Building Our Recipes List

通过templete添加列表

## 13 - Template Level Subscriptions



## 14 - FlowRouter Parameters



## 15 - Single Item Subscriptions

## 16 - User State Redirects in Routing

## 17 - Login & Logout Redirecting

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

##18 - Update Methods & Adding To Menu

##19 - Filtering Our In Menu Items

通过style的设置巧妙的解决不同状态下显示不同button的问题

##20 - Each:Else for No Results

通过另外一种方式设置不同状态下不同button的显示问题

##21 - Building The Shopping List


##22 - Updating With A QuickForm

autosave是个好功能

##23 - Deleting Recipes and Session Helpers

