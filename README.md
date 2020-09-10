# bdmap-moTzxx

- 背景

	最近鄙人在使用富文本编辑器时发现：
	[ ***`Tiny 中文文档`***](http://tinymce.ax-z.cn/more-plugins/bdmap.php) 提供的百度地图插件并不好用；
	无法达到基本的搜索匹配、放大缩小、拖拽等基本功能；
	存在着代码报错，推测是测试不够严谨，于是在此基础上进行优化，欢迎指摘 ...

- 优化后效果：

	①. 对输入框实现了 `"input propertychange()"` 监听事件
	②. 设计地址下拉框展示效果
	③. 即时获取 `百度地图服务器` 返回的匹配地址数据
	④. 触发点击事件及搜索定位优化
	> 优化后效果截图如下：
![](https://img-blog.csdnimg.cn/202009091833583.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3UwMTE0MTU3ODI=,size_16,color_FFFFFF,t_70#pic_center)
- 使用指导
	直接替换原来的 `“plugins/bdmap"` 文件夹即可 (本身来讲就是增加了一些逻辑代码)
![](https://img-blog.csdnimg.cn/20200909185055972.jpg?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3UwMTE0MTU3ODI=,size_16,color_FFFFFF,t_70#pic_center)

- 附录
>`【建议】`
  1  推荐参考： [***百度地图 Javascript API 开发指导***](http://lbsyun.baidu.com/index.php?title=jspopular3.0)
>2 注册自己的 百度地图开发 应用账号,"map.html"中的是我自己注册的AK值，仅做小范围应用
```js 
<script charset="utf-8" src="http://api.map.baidu.com/api?v=3.0&ak=M7GFlg9ApjGlQDFh8gHDaxxzLu7KfuSc"></script>
```
>`【源码】`
可自行深度优化： [ ***`>>>源码下载地址 GitHub >>>`***]()
