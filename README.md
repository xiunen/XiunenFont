XiunenFont
==========

一款百度常用logo的字体

如何使用XiunenFont
------------------------------
1 下载XiunenFont字体，假设放在webroot下的 fonts下面

2 css @font-face引入字体，引入代码如下：
		@font-face {
			font-family: 'xiunen';
			src: url('fonts/xiunen.eot');
			src: local('☺'), url('fonts/xiunen.woff') format('woff'), url('fonts/xiunen.ttf') format('truetype'), url('fonts/xiunen.svg') format('svg');
			font-weight: normal;
			font-style: normal;
		}

3 使用其中的字体，现在提供了10个字，对应的字和class如下：

![github](https://github.com/xiunen/XiunenFont/icon.jpg "github")  

如何制作自己的字体
-----------------------------
1 下载字体制作软件 FontCreator

2 新建字体，给字体取名字

3 删除所有默认字体

5 配置默认值：格式->设置->范围，设置x高度:0, 大写高度:0

6 空白处右键点击“添加”，会展开画布

7 工具->导入图像。然后调整图像，最后生成字体。

8 剪切轮廓工具修剪掉多余的东西

9 右键->属性；常规设置postscript名称；

设置映射：选择平台，添加或者选择对应的值，然后点击确定

10 为了web使用字体，到 http://www.font2web.com/ 生成字体文件

11 下载字体文件之后修改fonts.css，添加字体的映射。假设第9步设置的某个字的值是$F000, 那么在css中使用\f000来取到这个值。
