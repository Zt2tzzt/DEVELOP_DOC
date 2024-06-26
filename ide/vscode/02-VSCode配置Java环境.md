# 一、VSCode Java 环境配置

## 1.VSCode 插件安装

安装 VSCode 插件包 [Extension Pack for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)、[Spring Boot Extension Pack](https://marketplace.visualstudio.com/items?itemName=vmware.vscode-boot-dev-pack)。

插件安装完成后，资源管理器会多出一个“创建 Java 项目”的按钮。

- 或者使用 Ctrl + Shift + P，选择“创建 Java 项目”。
- 或者使用 F1，选择“创建 Java 项目”。

### 1.Java 项目创建

1. 使用 Ctrl + Shift + P，选择”创建 Java 项目“
2. 选择”No build tools“，创建一个不适用任何构建工具的 Java 项目。

### 2.构造方法，get、set 方法生成

右键 -> 源代码操作 -> Generate Constructors

右键 -> 源代码操作 -> Generate getter / setter

## 2.VSCode 代理设置

为 VSCode 设置代理，这样在创建 Java 项目时，可以更快的响应。

进入设置，搜索 `proxy`，然后设置 http proxy 为 `http://127.0.0.1:7890`。

## 3.VSCode maven 设置

在 VSCode 中，设置本地 maven 的全局配置：

- 进入“设置”，找到 `Maven: Global Settings` 的配置项，进行配置：
- 设置本地 maven 的 conf 目录下的 settings.xml 文件的绝对路径，即：`D:\Devtools\apache-maven-3.6.3\conf\settings.xml`

在没有设置 VSCode 代理的情况下，如果本地没有现成的依赖，那么项目构建加载 maven 依赖就会变得很慢，在 VSCode 中，对 maven 进行相关的设置。

- 进入“设置”，找到 `Maven: Executable: Path` 的配置项，进行配置；
- 设置本地 maven 目录下的 bin 目录绝对路径。即 `D:\Devtools\apache-maven-3.6.3\bin`。

### 1.maven 项目创建

在 VSCode 中，创建一个 maven 项目：

1. 使用 Ctrl + Shift + P 打开命令窗口，选择”创建 Java 项目“
2. 选择”maven“，创建一个基于 maven 的 Java 项目。
3. 选择”maven-archtype-quickstart“后者”archtype-quickstart-jdk8“
4. 选择 maven 的版本号；
5. 输入项目名称。并选择项目创建的路径。
6. 等待 maven 项目构建。
7. 输入项目版本号。
8. 确认属性配置。

打开项目中的 pom.xml 文件，添加一个依赖：

1. 使用 Ctrl + Shift + P 打开命令窗口，选择”Maven: 添加依赖“。
2. 输入一个 maven 依赖名称，比如：`mysql`；
3. 任意选择一个具体的依赖。比如：`mysql-connector-java`；
4. VSCode 会提示 build file 已经修改，是否要重新构建项目，点击是。
5. 点击右方”JAVA PROJECT“ -> ”Maven Dependencies“，查看 jar 包是否有加载出来。

### 2.JavaWeb 项目创建

下载 VSCode 插件 Tomcat for Java（已弃用，[Community Server Connectors](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-community-server-connector) 代替）。

下载 XML 插件，xml，xml tool

## 4.VSCode 运行和调试设置

步骤如下：

1. 将侧边菜单栏，切换至”行和调试“，点击创建 `launch.json` 文件；
2. 将侧边菜单栏，切换至“资源管理器”，打开`.vscode` 文件夹下的 `launch.json`；
3. 如图所示添加`"console": "externalTerminal"`，并保存。
