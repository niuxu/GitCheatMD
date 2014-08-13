#Winlab的[Cmd Markdown](https://www.zybuluo.com)大法
标签（空格分隔）： Markdown Cheat
---
###1.斜体和粗体
用\*和\**表示斜体和粗体
eg:
这是*Winlab*， 这是 **Winlab** 
###2.分级标题
用===表示一级标题，----表示二级标题
```
这是一级标题
==================
这是二级标题
------------------
###这是三级标题
```
当然行首加#也能表示不同级别标题(H1-H6),如# H1, ##H2, ###H3
###3.超链接
使用\[描述](连接地址)添加超链接
eg:
通向[Winlab](http://winlab.ustc.edu.cn)的大门
###4.无序列表
使用*,+,-表示无序列表
eg：

- 218室
- 219室
- 222室

###5.有序列表
数字+'.'

1. 球机1
2. 球机2
3. 球机3

###6.文字引用
使用>表示文字引用
eg：
>let's talk about massive mimo

###7.行内代码块
使用\`代码\`表示行内代码
eg：How to learn `C++` in 21 days
###8.代码块
使用 四个缩进空格 表示代码块
eg：

    cout<<"吃了吗"<<endl;
###9.插入图像 
使用\!\[描述](图像连接地址)插入图像
eg:
![Winlab的头像](http://winlab.ustc.edu.cn/winlab/Tpl/default/Public/images/logo.jpg)

#Cmd MarkDown高阶指南
###1.内容目录
在段落中添加`[TOC]`显示全文内容的目录

[TOC]
###2.标签分类
在编辑区任意行首位置加入代码来给文稿加标签

标签 : 王老板 卫老板 陈sir
或
Tags : 王老板 卫老板 陈sir
###3.删除线
使用 ~~ 表示删除线
~~陛下臣有罪~~
###4.注脚
使用[^keyword]表示注脚，注脚之间加入空行才会识别
eg:
Winlab有三好[^footnote]。

史上最大交友网站[^footnote1]
###5.LaTeX公式

\$  表示行内公式：
香农公式 $C=B*log2(1+S/N) $。
\$\$表示整行公式:
$$I(X,Y)=H(X)+H(Y)-H(X,Y)$$
$$F(\color{maroon}\omega)=\mathscr{F}[f(t)]=\int_{-\infty}^\infty f(t)e^{-i\omega t}dt$$
访问[MathJax](http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference)来完善你的公式
###6.加强的代码块
支持行号显示和语法高亮
非代码示例
```
$mkdir rocky
```
C++示例
```
void swap(int &a, int &b)
{
    if(a != b)
    {
        a ^= b;
        b ^= a;
        a ^= b;
    }
}
```
###7.流程图
示例（：后需加入空格）
```flow
st=>start: start:>http://winlab.ustc.edu.cn
io=>inputoutput: verification
op=>operation: Your Operation
cond=>condition: Yes or No?
sub=>subroutine: Your Subroutine
e=>end

st->io->op->cond
cond(yes)->e
cond(no)->sub->io
```
[语法参考](http://adrai.github.io/flowchart.js)

###8.序列图
示例1 seq必须在```后
```seq
BossWang->Yange: 怎么样了
Note right of Yange: 颜哥急中生智ing
Yange->BossWang: 尹sir找我有事
```
示例2
```seq
Title: Winlab大事记
A->B: Normal line
B-->C: Dashed line
C->>D: Open arrow
D-->>A: Dashed open arrow
```
[语法参考](http://bramp.github.io/js-sequence-diagrams/)

###9.表格
示例

| 名字   | 项目   | 价格 |
|--------|:------:|:----:|
|   夏老湿  |   洗剪吹 |   0  |
|   颜总    |   只卖艺 |    2   |
|   文爽    |   肥皂舞  |   -2  |
###10.定义型列表
名词1
:    定义1（冒号+四个空格）

代码块2
:    代码块的定义(冒号+四个空格，注意代码块2上需要空行)

        代码块(左侧8个空格，上面空行)

###11.Html标签
支持在Markdown语法中嵌入Html标签，如用Html写一个表格

    <table>
        <tr>
            <th rowspan="2">扫地人员</th>
            <th>2012</th>
            <th>2013</th>
            <th>2014</th>
        </tr>
        <tr>
            <td>酋长</td>
            <td>酋长</td>
            <td>酋长</td>
        </tr>
    </table>

<table>
    <tr>
        <th rowspan="2">扫地人员</th>
        <th>2012</th>
        <th>2013</th>
        <th>2014</th>
    </tr>
    <tr>
        <td>酋长</td>
        <td>酋长</td>
        <td>酋长</td>
    </tr>
</table>
###12.内嵌图标
文档输入

    <i class="icon-apple"></i>
    
显示小苹果: <i class="icon-apple icon-2x"></i>
显示小企鹅: <i class="icon-linux icon-2x"></i>
图标说明[font-awesome](http://fortawesome.github.io/Font-Awesome/3.2.1/icons/)

[^footnote]:基友多，基友多，基友多。

[^footnote1]:www.stackoverflow.com
