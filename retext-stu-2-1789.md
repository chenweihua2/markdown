### 1.标题字体大小等级，这个最简单了，幼儿班课程

# 1
## 2
### 3
#### 4
##### 5
###### 6

1：with =，就是在下一行敲三个=
===

2：with -，就是在下一行敲三个-
---

### 2.段落，可以用Tab

这是一个段落。如果要换行，敲两个空格回车。  
这就是第二行。

    这里用了Tab，看看什么样式？怎么没变化呢？到了后面才知道这一行已经取消格式，也就是说保持输入时的样式没有格式化
    这里用了四个空格，看看什么样式？也没变化，只是在编辑状态下回车下一行时，会自动缩进而已！

### 3.强调：如，加粗、倾斜、删除……

这是**加粗**样式，这是*倾斜*样式，这是~~删除~~样式。

### 4.列表

#### 无序列表，用-加空格
- name：阿弥陀佛
    - 弟子：大势至菩萨
    - 弟子：观世音菩萨
- age：多劫
- XB：佛，无性别，三十二相，八十种好
- work：西方极乐世界教主

#### 有序列表
1. name：释迦牟尼佛
    1. 弟子：憍陈如尊者
    2. 弟子：阿难尊者
2. age：三千多年，其实不是，和阿弥陀佛一样
3. XB：佛，紫磨真金色身
4. work：社会多元文化教育工作者

### 4.链接，提倡多用引用式链接

#### 非引用式链接，内嵌式链接

- 外部链接：[佛学视频](http://www.fxsp.org/)
- 内部链接1，链接仓库其他的文件：[README](README.mkd)
- 内部链接2，链接本文档的其他部分：[dmk](retext-stu-2-1789.md#7.代码块)

#### 引用式链接

- 外部链接：[佛学视频]
- 外部链接：[佛学视频][fxsp]
- 内部链接1，链接仓库的其他文件：[README]
- 内部链接2，链接本文档的其他部分：[代码块]

### 5.图片，这里也和链接一样，只是写法多了在句首多了一个感叹号!

#### 内嵌式链接

    ![alt](url text)，alt和text可以缺省

- 外部图片，即远程其他主机的图片：![](http://zhaojing.ren/content/uploadfile/201701/top-1485165584.jpg)
- 本地图片，即本地自己主机的图片：![zhaojing](images/top-1485165584.jpg)

#### 引用式链接

- 外部图片，即远程其他主机的图片：![zhaojing][pic_remote]
- 本地图片，即本地自己主机的图片：![zhaojing][pic_local]

### 6.引用

> 这是一个引文。

>>> ——这是一个多重引文（在格式上可以写引文出处）。

### 7.代码块

- 行内代码

这个代码中用来声明变量是`var a = 10`，打印变量内容是`consloe.log`函数的调用。

- 块式代码

```javascript

var a=999;
console.log(a);

```
### 8.水平分割线，用-、*、_，这三个符号，<hr> Horizontal Rule

---
***
___


### 9.HTML 代码，这个需要学习一点HTML的知识

<p align="center">
阿弥陀佛！
</p>
<p align="center">
<img src="images/top-1485165584.jpg">
</p>

### 10.表格，这个很有用


|表头1默认靠左|表头2居中|表头3靠右|
|------------|:---------:|------------:|
|律|经|论|
|弘一法师|佛说大乘无量寿庄严清净平等觉经|大智度论|
|[佛学视频]|[zhaojing]|[README]|

### 11.GFM，GitHub Flvored MarkDown，GitHub特有MarkDown样式

task

- [x] item1
- [ ] item2
- [x] item3

### 12.表情符号

:snake:

## 总结进阶
### 13.混合强调样式

- ***加粗倾斜***
- **~~加粗删除~~**
- *~~倾斜删除~~*
- ***~~加粗倾斜删除~~***

### 14.图片链接

基本文字链接

![pic_remote](http://zhaojing.ren/content/uploadfile/201701/top-1485165584.jpg)

基本图片

图片链接

[![pic_remote]][zhaojing]

### 15.引用链接的问题

基本引用链接的用法：

good：  
[照镜人][zhaojing]  
[抑郁之家][zhaojing]

low:  
[照镜人](http:zhaojing.ren)  
[抑郁之家](http:zhaojing.ren)


### 16.多级有序列表

问题1：如何打断，这里一定要有文字段落（空行不行）才能把有序列表打断，底下的3序号就变成1了

1. item 1
	1. item 1.1
	2. item 1.2
2. item 2


fdsafdsafdsafdsafd

fdsafdsafdsafdas





3. item 3
4. item 4

<!-- 以下是引用链接 -->
<!-- 存在几个问题，有序列表不能打断；图片链接地址后面加别名不行；文档内跳转不行-->
[佛学视频]:http://www.fxsp.org
[fxsp]:http://www.fxsp.org
[README]:README.md
[代码块]:retext-stu-2-1789.md#7.代码块

[pic_local]:images/top-1485165584.jpg
[pic_remote]:http://zhaojing.ren/content/uploadfile/201701/top-1485165584.jpg
[zhaojing]:http://zhaojing.ren
