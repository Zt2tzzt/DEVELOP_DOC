# IDEA 快捷键

## 一、便携操作

Shift + F6，重命名（类名，变量名，方法名）。

F2 / Shift + F2，定位下一个/上一个错误。

Ctrl + Z / Ctrl + Shift + Z，撤销 / 反向撤销；

Ctrl + Alt + V，生成等号左边的代码。

Ctrl + Shift + \，分屏（自定义的快捷键）

Ctrl + B / Ctrl + 左键，跟进原码。

Ctrl + Alt + ←/→，切换页签

Ctrl + E，打开关闭的页签。

## 二、注释

Ctrl + /，行注释。

Ctrl + Shifr + /，代码块注释

/** + Enter，在要生成文档注释的方法上，生成文档注释。

## 三、格式化

Ctrl + Alt + Shift + L（大写），格式化代码，可以对当前文件和整个包目录使用。

Shift + Tab，取消缩进。

## 四、段落操作

Ctrl + [ / ]，回到光标所在括号开头/结尾；

Ctrl + W，光标移动到括号开头，选中括号中的内容。

## 五、多行操作

Alt + 鼠标左键拖动，选中连续的多行进行编辑。

Alt + Shift + 鼠标左键点击，选中单个的多行进行标记

逐行递增数字：下载插件 [String Manipulation](https://plugins.jetbrains.com/plugin/2162-string-manipulation)，选中多行要递增的数字，Alt + M，increment/decrement，increment

## 六、行操作

### 1.删除行

【Windows】Ctrl + Y；【Mac】Command + BackSpace，删除光标所在行 或 删除选中的行

### 2.移动行

Shift + Alt + ↑/↓，向上/下移动当前行。

### 3.复制行

Ctrl + C，复制光标所在行。或复制选择内容。

Ctrl + D，复制光标所在行，或复制选择内容，并把复制内容插入光标位置下面

### 4.换行

Shift + Enter，在当前行下方开始新行，

Ctrl + Alt + Enter（⌥ + ⌘ + Enter ），在当前行上方开始新行，

### 5.缩进

Shift + Tab，缩进、取消缩进。

## 七、单词操作

### 1.选中单词

【Windows】 ：Ctrl + W；【Mac】Opt + ⬆️；选中光标所在的单词

【Windows】：Alt + j；【Mac】：Ctrl + G；选中下一个相同的单词；

Ctrl + Shift + Alt + j，选中所有相同的单词

Ctrl + Shift + U / L，将选中的单词大写。

## 八、方法操作

Ctrl + P，调用方法时，把光标移动到括号里，按下快捷键，查看方法传参顺序。

Ctrl + Alt + M，选中要抽取的方法体，按下快捷键，自动抽取代码。

Alt + Enter，根据方法调用语句生成方法。

## 九、类操作

【Windows】Alt + insert；【Mac】Com + N；为 JavaBean 类创建构造方，getter、setter 访问器等等。

- 按两下 Tab，再按 Enter，表示不选中任何选项，通常用于创建空参构造方法。

Alt + 7，罗列类中的成员。

Ctrl + F12，展示类中所有方法。

- 黄色 f（field）开头的是成员变量，或者常量。
- 蓝色 c（class）开头的是内部类。
- 绿色 i（interface）开头的是接口。
- 红色 m（method）开头的是方法；
  - 后方有类似于"↑ Xxx"的灰色字体，表示重写了 Xxx父类中的方法。
  - 灰色的方法体，并且后方有类似于“→ Xxx”，表示是继承的 Xxx 父类中的方法。

Ctrl + O，重写类中的方法。

## 十、变量操作

Alt + Enter，变量和赋值语句进行切割。

## 十一、代码块操作

Ctrl + Shift + -，一次性折叠所有代码块。

Ctrl + Shift + +，一次性打开所有代码块

Ctrl + -，折叠光标所在代码块。

Ctrl + +，打开光标所在代码块。

Ctrl + Alt + T，选中代码，选择用什么语句体包裹。

## 十二、搜索、查找、替换

Shift * 2，全局查找文件。

【Windows】Ctrl + N；【Mac】Com + O 根据输入的类名查找类文件 `（必备）`

【Windows】Ctrl + Shift + N；【Mac】Com + Shift + O 根据输入的文件路径查找类文件 `（必备）`

Ctrl + F，搜索文件。

Ctrl + R，替换文件搜索到的内容。

Ctrl + Shift + F，搜索项目。

Ctrl + Shift + R，替换项目搜索到的内容。
