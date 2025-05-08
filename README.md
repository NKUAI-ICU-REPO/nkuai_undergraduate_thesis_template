# 欢迎使用nkuai本科生毕业设计typst模板

### Why Typst？

typst是一种不同于Microsoft Word和$L^AT_EX$的排版系统，它拥有着足以媲美$L^AT_EX$的高度定义排版方式，$L^AT_EX$同款的优美数学公式字体，不会像Microsoft Word那样找不到隐形的“空格”，莫名的空白换行符换页符。同时，相比于$L^AT_EX$，typst具有更加高效的编译速度以及更容易上手的排版语法。

### 使用须知

本模板仅适用于南开大学人工智能学院的本科生毕业设计论文，不能保证可以适用于其他单位的论文排版。另外，由于人工智能学院的排版要求反复无常，所以请各位在使用本模板的时候注意以当年的要求为准。

另外，本模板没有制作声明页，因为这一页后续还需要签名，建议先把声明页导出为pdf之后签名然后在[線上整理PDF文檔。](https://www.ilovepdf.com/zh-tw/organize-pdf)直接插入声明页到最终的论文中。

### 免责声明

模板中的字体文件并非本人的成果，演示用的实验图片来自Harvard公开的医学影像数据集，Restormer的模型图片是本人绘制的。**模板中的所有段落均已脱敏，仅为演示用，没有任何意义**。另外部分代码借鉴了[东南大学的typst论文模板](https://github.com/csimide/SEU-Typst-Template)，非常感谢这些来自SEU的开发者。算法块的实现改自[GitHub - lf-/typst-algorithmic: Algorithm pseudocode typesetting library for Typst](https://github.com/lf-/typst-algorithmic/tree/main)

### 如何使用本模板

`clone`该仓库到本地即可开始编译使用。非常建议使用vscode的Tinymist Typst进行编辑。另外注意，本模板使用的字体都可以在`fonts/`下找到，如果你的typst在编译的时候遇到字体无法正常显示的问题，按需从字体文件夹中安装。

> 理论上来说，typst是可以使用本地字体文件的，但是Tinymist Typst似乎没法直接使用指定文件夹下的字体文件包括`.ttf`和`.otf`。（Tinymist的官方说法是在插件设置文件中指定`"tinymist.fontPaths"`的键值，但是作者指定了似乎也没有用）不过只要系统安装了对应的字体那么就应该可以正常编译。
> 
> 作者的在linux上使用自定义字体的实践方法是：
> 
> 1. 找到你想要的字体文件，放入到`/usr/share/fonts/`下
> 
> 2. 给予该字体`777`权限
> 
> 3. Tinymist的设置文件中，添加`"tinymist.preview.cursorIndicator": true`
> 
> Windows上尚未实践。

本模板一个正确的章节书写方式

```typst
#set-heading-1("第一章 哈基米")//这个函数用于控制当前也开始之后的页眉内容
#set-heading-seq(2)//这个用来控制编号，第n章就传入n作为参数
#clear-local-image-seq()
#clear-local-table-seq()//这两个函数与#set-heading-seq用于控制章节内的图表编号
#pagebreak()//分页符，一定要在上面几个函数之后调用

= 第一章 哈基米//一级标题要手动把章节的编号写出来
峹衁攍蓯甒朦喬泔纙彴鮹妱遞肐姇匌眝皑窧凿獛佤誨弹駕熥岹放珂仸養嗐慗惎鳊，鸎撡炒牞抸磀噫辆璈煬獅矿颒萦昕檺腖甔盹婈蕦樔禡蜒药超。

#end-of-section()//每一段文字写完之后，要加上这个用于实现word模板的分节

== 第一节 哈基米哈气

卣析糧朅膣嬸椀邎儦拗謱硯访擲钿潈覃。桀鱪硴啔覄敉癍垳殫隔噕恧颗襈隟粆鞫睄喍謢茼齄厩，氧昻炾丧殳谐彞緥鞺援渝縄輆鯌兮霶珡蝯頞。

#end-of-section()

=== 三级标题并不需要写序号本模板自动编号

霪讄門鍠栵瞦缡箢乩愖穴堧瓋盽。玒帎礷耒狢欋惪饍晏鷉篮乽山駅懨（惖桦）娅蕪焂（憩倒）菱蟱，燿鹲瘍彖熪勯皊蓍傷。

#end-of-section()
```

关于图表的使用，可以参考模板中的例子



### typst基本语法快速上手

https://typst.app/docs/tutorial/writing-in-typst/



### 项目目录

```text
.
├── algorithmic.typ//算法块
├── cite.bib//引用文件，bibtex格式
├── fonts//字体文件夹，按需安装
├── fonts.typ//各种字体函数
├── gb-t-7714-2015-numeric.csl//改动的国标应用文件以适应学院模板要求
├── img//图床
├── README.md
├── refs//官方的模板
├── thesis.pdf//导出示例
└── thesis.typ//主模板

```






