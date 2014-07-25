TEST
===========================
This README.md is used to test all kinds of syntax of GitHub Flavored Markdown.
---------------------------
###　　　　　　　　　　　　Author:Jelly
###　　　　　　　　　 E-mail:879231132@qq.com

===========================



##<a name="index"/>目录
* [横线](#line)
* [标题](#title)
* [显示文本](#text)
    * 普通文本
    * 单行文本
    * 多行文本
    * 部分文字高亮
* [超链接](#link) 
    * 文字超链接
        *  链接外部URL
        *  链接本仓库里的URL
        *  锚点
    * [图片超链接](#piclink)
* [显示图片](#pic)
    * 来源于网络的图片
    * GitHub仓库中的图片
* [列表](#dot)
* [缩进引用](#symbol)
* [代码高亮](#code)
* [显示表格](#table) 

<a name="line"/>
##***、---、___显示虚横线
***
---
___



<a name="title"/>
#一级标题
##二级标题
###三级标题
####四级标题
#####五级标题
######六级标题


##<a name="text"/>显示文本
###普通文本
这是一段普通的文本，
直接回车不能换行，<br>
要使用\<br>

或者就是在两段文本直接加一个空行。

也能实现换行效果，不过这个行间距有点大。
###单行文本
    Hello,大家好，我是果冻虾仁。
###多行文本
    欢迎到访
    很高兴见到您
    祝您，早上好，中午好，下午好，晚安
###部分文字高亮
Thank `You` . Please `Call` Me `Coder`
####高亮功能更适合做一篇文章的tag
例如:<br>
`java` `网络编程` `Socket` `全双工`
####删除线
这是一个 ~~删除线~~
####斜体
*斜体1*

_斜体2_
####粗体
**粗体1**

__粗体2__


##<a name="link"/>文字链接
###链接外部URL
[我的博客](http://blog.csdn.net/guodongxiaren/article/details/23690801 "悬停显示")
###链接的另一种写法
[我的博客][1]
[1]:http://blog.csdn.net/guodongxiaren/article/details/23690801 "悬停显示"
>中括号[]里的id，可以是数字，字母。这两行可以不连着写，一般把第二行的链接统一放在文章末尾，id上下对应就行了。这样正文看起来会比较干净。

###链接本仓库里的URL
[Book](./Book)
###锚点
[点此回到目录](#index)

##<a name="pic"/>显示图片
###来源于网络的图片
![baidu](http://www.baidu.com/img/bdlogo.gif "百度logo")
###GitHub仓库中的图片
![](https://github.com/guodongxiaren/ImageCache/raw/master/Logo/foryou.gif)
###<a name="piclink">给图片加上超链接
[![head]](http://blog.csdn.net/guodongxiaren/article/details/23690801)
[head]:https://github.com/guodongxiaren/ImageCache/raw/master/Logo/jianxin.jpg "点击图片进入我的博客"

##<a name="dot"/>列表
###圆点列表
* 昵称：果冻虾仁
* 别名：隔壁老王
* 英文名：Jelly

###更多圆点
* 编程语言
    * 脚本语言
        * Python

### 复选框列表
- [x] C
- [x] C++
- [x] Java
- [x] Qt
- [x] Android
- [ ] C#
- [ ] .NET

##<a name="symbol"/>缩进
###用于列表
>数据结构
>>树
>>>二叉树
>>>>平衡二叉树
>>>>>满二叉树

###用于引用：
####文本摘自《深入理解计算机系统》P27
　令人吃惊的是，在哪种字节顺序是合适的这个问题上，人们表现得非常情绪化。实际上术语“little endian”（小端）和“big endian”（大端）出自Jonathan Swift的《格利佛游记》一书，其中交战的两个派别无法就应该从哪一端打开一个半熟的鸡蛋达成一致。因此，争论沦为关于社会政治的争论。只要选择了一种规则并且始终如一的坚持，其实对于哪种字节排序的选择都是任意的。
><b>“端”（endian）的起源</b><br>
以下是Jonathan Swift在1726年关于大小端之争历史的描述：<br>
“……下面我要告诉你的是，Lilliput和Blefuscu这两大强国在过去36个月里一直在苦战。战争开始是由于以下的原因：我们大家都认为，吃鸡蛋前，原始的方法是打破鸡蛋较大的一端，可是当今的皇帝的祖父小时候吃鸡蛋，一次按古法打鸡蛋时碰巧将一个手指弄破了，因此他的父亲，当时的皇帝，就下了一道敕令，命令全体臣民吃鸡蛋时打破较小的一端，违令者重罚。”


##<a name="code"/>代码高亮
```Java
public static void main(String[]args){} //Java
```
```c
int main(int argc, char *argv[]) //C
```
```Bash
echo "hello GitHub"#Bash
```
```javascript
document.getElementById("myH1").innerHTML="Welcome to my Homepage"; //javascipt
```
```cpp
string &operator+(const string& A,const string& B) //cpp
```
##<a name="table"/>显示表格
First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |

| Name | Description          |
| ------------- | ----------- |
| Help      | Display the help window.|
| Close     | Closes a window     |

表格中也可以使用普通文本的删除线，斜体等效果

| Name | Description          |
| ------------- | ----------- |
| Help      | ~~Display the~~ help window.|
| Close     | _Closes_ a window     |

表格可以指定对齐方式

| Left-Aligned  | Center Aligned  | Right Aligned |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |
