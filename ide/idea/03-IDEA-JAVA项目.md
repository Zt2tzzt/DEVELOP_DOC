# IDEA java 项目

## 一、IDEA Java 项目结构

IDEA Java 项目结构分为四类：

### 1.project（项目、工程）

project（项目、工程）是 IDEA 的最外层层级。它的下一层是 module（模块）。

### 2.module（模块）

在一个 project（项目、工程）中，可以存放多个模块，比如：

- 论坛模块；
- 报名、咨询模块。

为了更好的管理代码，项目中不同的业务功能代码，存放在不同的模块中。

### 3.package（包）

一个 module（模块）中又有很多的业务，以一个项目的论坛模块为例，至少包含了以下不同的业务。

- 发帖
- 评论

每一块业务，存放在一个 package（包）中。

### 4.class（类）

package（包）中存放了若干 class（类）。

class（类）是真正写代码的地方。

![IDEA项目解构](NodeAssets/IDEA项目解构.jpg)

## 二、IDEA 创建一个空 Java 项目

### 1.project（项目、工程）创建

打开 IDEA 开发工具，创建一个 project（项目、工程）

1. 点击“New Project”；
2. 点击右侧“Empty Project”。
3. 为项目起名，并选择项目存放位置

### 2.module（模块）创建

为这个项目，创建一个 module（模块）

1. 点击左上角“File”，再点击“Project Structures”；
2. 在弹出的窗口右侧，选择“Modules”，点击窗口上方“+”号。再选择“New Modules”；
3. 选择左侧“JAVA”，表示新建一个 JAVA Module；并为 module（模块）起名。
4. 点击下方“OK”，创建 module（模块）。

#### 1.module（模块）导入

为这个项目，导入一个已存在的 module（模块）；

1. 点击左上角“File”，再点击“Project Structures”；
2. 在弹出的窗口右侧，选择“Modules”，点击窗口上方“+”号。再选择“Import Modules”；
3. 选择已有模块（Module）目录下的 `.iml` 配置文件。
4. 点击下方“OK”，导入 module（模块）。

#### 2.第三方（jar）包导入

1. 在 module 模块中，创建一个目录 `lib`，将第三方包 `xxx.jar` 放在该目录下。
2. 右键该第三方包，选择“Add as Library”。

### 3.package（包）创建

在模块中，新建一个 package（包），本质上就是一个文件夹（目录）：

1. 选中右侧菜单中 module（模块）下的 src 目录，右键 -> New -> Package。
2. 为 package（包）命名，习惯以公司域名的反写，加上 package（包）名来命名；
   - 比如：公司域名的反写是：`com.kkcf`；包名是 `demo01`；加起来就是 `com.kkcf.demo01`；
   - 这个步骤，本质上是在 `src` 目录下，新建了一个 `com` 文件夹，在它下面又新建了一个 `kkcf` 文件夹，在它下面又新建了一个 `demo01` 文件夹；

### 4.class（类）创建

在 package（包）中，新建一个 class 类。

1. 在右侧项目目录结构中，选中刚刚创建的 package（包），右键 -> New -> Java Class；
2. 为 class（类）取名（注意遵守 class 类的命名规范）；
3. 选中“class”，回车。

#### 5.interface（接口）创建

在 package（包）中，新建一个 interface 接口。

1. 在右侧项目目录结构中，选中刚刚创建的 package（包），右键 -> New -> Java Class；
2. 为 interface（接口）取名（注意遵守 class 类的命名规范）；
3. 选中“interface”，回车。

## 三、IDEA 类、模块、项目操作

### 1.IDEA class（类）的操作

我们知道，在项目中，每一个 .java 文件，就是一个 class 类。

**新建 class 类**；在 package（包）中，新建一个 class 类的步骤如下：

1. 在右侧项目目录结构中，选中刚刚创建的 package（包），右键 -> New -> Java Class；
2. 为 class（类）取名（注意遵守 class 类的命名规范）；
3. 选中“class”，回车。

**修改 class 类**；在 package（包）中，修改一个 class 类的类名，步骤如下：

1. 在右侧项目目录结构中，选中要修改的 .java 文件；
2. 右键 -> Refactor > Rename。
3. 输入修改的名称，回车。

**删除 class 类**；在 package（包）中，删除一个 class 类的步骤如下：

1. 在右侧项目目录结构中，选中要删除的 .java 文件，右键 -> delete。

### 2.IDEA module（模块）的操作

**新建 module 模块**；为这个项目，创建一个 module（模块）

1. 点击左上角“File”，再点击“Project Structures”；
2. 在弹出的窗口右侧，选择“Modules”，点击窗口上方“+”号。再选择“New Modules”；
3. 选择左侧“JAVA”，表示新建一个 JAVA Module；并为 module（模块）起名。
4. 点击下方“OK”，创建 module（模块）。

修改 module 模块

删除 module 模块

导入 module 模块

### 3.IDEA project（项目、工程）操作

**关闭 project 项目**；关闭当前打开的项目：

1. 点击左上角“File”，再点击“Close Project”；

**新建 project 项目**；打开 IDEA 开发工具，创建一个 project（项目、工程）

1. 点击“New Project”；
2. 点击右侧“Empty Project”。
3. 为项目起名，并选择项目存放位置。

打开项目

修改项目
