## 什么是AMP?
> AMP(Accelerated Mobile Pages) 移动页面加速，是Google启动的一个加快移动页面加载速度的项目。

个人理解而言属于一套页面编写规范，比如就官网解释的运作原理做介绍。  
1. 仅允许异步脚本
```
  JavaScript或阻塞DOM的构建，延缓页面渲染，所以AMP仅允许使用异步JavaScript。
  AMP页面不能包括作者自己编写的任何JavaScript，使用自定义AMP元素来出炉互动页面功能。
```
2. 静态确定所有资源的大小
```
  图片、广告或iframe等外部资源必须在HTML中声明其大小，一遍AMP可以再下载前确认每个元素的大小和位置。
  AMP不需要等待所有资源下载完成就可以直接加载页面布局
```
像以上的两条就属于AMP的运作原理，基于此原理，AMP开发出了一套自己的组件，如amp-img代替img等，从而实现对页面的优化，加速页面渲染。

[demo](./index.amp.html)  
**[官网介绍](https://www.ampproject.org/zh_cn/learn/about-how/)**

