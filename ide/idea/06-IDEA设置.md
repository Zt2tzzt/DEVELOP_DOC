# IDEA 设置

## 1.进入 IDEA 的设置界面

1. 点击上方“File”，再点击“Settings”。

## 2.设置主题

1. 选择右侧“Appearance & Behavior”，再点击“Appearance”进行设置。

## 3.设置字体

1. 选择右侧“Editor” -> “Font”

## 4.设置自动导包

1. 选择右侧“Editor” -> “General” -> "Auto Import"
2. 勾选“Add umambiguous imports on the fly"和"Optimize imports on the fly"

## 5.设置代码提示忽略大小写

1. 选择右侧“Editor” -> “General” -> “Code Completion”；
2. 取消勾选“Math case”。

## 6.设置编辑工具的背景图片

1. 选择右侧“Appearance & Behavior” -> “Appearance” -> 点击“BackGround Image”；
2. 选中本地的一张图片，调整透明度即可。

## 7.设置项目单击打开文件、展开文件夹

1. 点击项目工作目录上方三个竖点（options），
2. 选择“Open File With Single Click”和“Open Directories With Single Click”

## 8.设置项目 JDK

1. 点击左上角“File”，再点击“Project Structures”；
2. 点击右侧“SDKs"，点击上方”+“号，再点击”Add JDK“。

### 8.1 选择项目编译的 JDK

1. 点击左上角“File”，再点击“Project Structures”；
2. 选择右侧“Project"，再选择右侧“language level”中对应的版本。

## 9.设置光标处逐行递增

1. 安装插件 [String Manipulation](https://plugins.jetbrains.com/plugin/2162-string-manipulation)；
2. 多光标选中要改变的值。
3. 按下 Alt + m，选择 Increment/Decrement，选择 Create Squeece。

## 10.设置 JavaBean 类序列化固定版本号

1. File -> Settings -> 搜索“Serializable”关键字
2. 勾选“Serializable class without 'serialVersionUID'”;
3. 勾选“Transient field is not initialized on deserialization”
