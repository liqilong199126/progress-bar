# progress-bar
常用的网页加载进度条
随着HTML5的普及，各种CSS3动画及JS特效在网页中层出不穷，PC端载入数据的速度还算可以，移动端相对要慢很多，如果图片或脚本没有完全载入，用户在操作中可能会发生各种问题，因此我们需要对数据载入进行侦测，以更加人性化的方式给用户展现。

## 通过加载状态事件制作进度条

- document.onreadystatechange 页面加载状态改变时的事件
- document.readyState 
返回当前文档的状态

1.uninitialized 还未开始加载

2.loading 载入中

3.interactive 已加载，文档与用户可以开始交互

4.complete 载入完成

## 实时获取加载数据的进度条

- 建立图像对象：图像对象名称=new Image（）
- 属性：border complete height...
- 事件：onload onerror onkeydown onkeypress...
- src属性一定要写到onload的后面，否则程序在IE中会出错
