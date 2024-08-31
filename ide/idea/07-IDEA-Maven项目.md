# IDEA Maven 项目

## 一、IDEA 集成 Maven 并创建 Maven 项目

IDEA 配置集成 Maven 有两种方案：

- 方案一：在当前项目（工程）project 中，集成 Maven。
- 方案二：创建一个 Maven 项目。

这里延时方案一的步骤，方案二的步骤与方案一类似，只是要将创建模块（module）改为创建项目（project）。

### 1.空项目集成 Maven

第一步，配置集成的 maven 安装路径

1. 进入 File  =>  Settings  =>  Build,Execution,Deployment  =>  Build Tools  =>  Maven。
2. 在右侧配置 Maven home path 作为集成的 maven 安装路径.
3. 手动指定 user settings file，将它设为 maven 安装目录下的 conf/settings.xml 配置文件的路径
4. IDEA 会加载该配置文件，并读取其中的本地仓库路径。

第二步，检查项目 maven 关联的 JRE 是否是要使用的版本：

1. 进入 File  =>  Settings  =>  Build,Execution,Deployment  =>  Build Tools  =>  Maven => Runner。
2. 在右侧配置 JRE 为当前想要使用的版本。

第三步，配置 Java 语言的字节码版本为要使用的版本。

1. 进入 File  =>  Settings  =>  Build,Execution,Deployment  =>  Compiler  => Java Compiler
2. 在右侧配置 project bytecode version 为想要使用的版本。

### 2.空项目中创建 maven 模块（module）

第一步，创建模块，选择 Maven ，点击 Next

1. 进入 Project Structure => Moudule => + 号 => New Module => java
2. 在右侧 Build system 选择 Maven。

第二步，填写模块名称，坐标信息，点击 finish，创建完成。

1. 在右侧打开 Advanced Setting，配置 GroupId，ArtifactId，version；它们分别表示组织名，模块名，版本号。这也被称为 maven 中的**坐标**。比如：

   - GroupId，设为 com.kkcf；

   - ArtifactId，设为 maven-01；

   - version 有 IDEA 自动生成，创建时无需指定。

2. 配置完成后，点击 Create 创建项目。maven 会自动加载项目所依赖的插件，放入本地仓库中。

3. 创建完成后，会发现 test 目录下，没有 resource 目录，这是因为它们不常用，需要的话要手动创建。

第三步，编写 HelloWorld，并允许。

demo-project/normal_project_with_maven/maven-01/src/main/java/com/kkcf/Test.java

```java
package com.kkcf;

public class Test {
    public static void main(String[] args) {
        System.out.println("Hello Project Module With Maven");
    }
}
```

在 IDEA 中，运行上面的代码，会发现项目目录结构中，多出了 target 目录，

## 二、IDEA 导入 Maven 项目

在 IDEA 中，导入 Maven 项目，操作路径：File -> Open -> 选中 Maven 项目下的 pom.xml 配置文件 -> Open as project.

在 IDEA 中，导入 Maven 模块，操作路径：File -> Project Structure -> + 号 -> Import Module -> 选中 Maven 项目下的 pom.xml 配置文件

## 三、IDEA 刷新 Maven 项目依赖

在 IDEA 中，右侧 maven 面板，查看 maven 项目目下是否有 `Dependencies`。如果没有，点击刷新来加载依赖。

## 四、IDEA 查看 Maven 依赖结构

在 IDEA 中，在 pom.xml 查看依赖结构步骤：

1. 进入 pom.xml 配置文件；
2. 右键 -> Diagrams -> Show Diagram

## 五、IDEA 执行 Maven 生命周期

在 IDEA 工具右侧的 maven 工具面板中，选择对应的生命周期，双击执行。

- 在 IDEA 中，执行某一生命周期阶段时，如果要跳过它前面的阶段，那么要选跳过的阶段，然后点击上方的”Skip Tests“图标。

在 IDEA 工具右侧的 maven 工具面板中，点开一个 Maven 项目，其中：

- `Lifecycle`，表示 Maven 的生命周期中的阶段；
- `Plugins`，表示执行 Maven 生命周期阶段所需要的插件。

## 六、IDEA 更新 Maven 依赖索引

有时候在 IDEA 配置完 maven 仓库信息后，依然搜索不到仓库中的 jar 包。

这是因为仓库中的 jar 包索引，尚未更新到 IDEA 中。这时，就需要更新 IDEA 中 maven 的依赖索引了，具体做法如下：

- Ssettings -> Build,Execution,Deployment  ->  Build Tools  ->  Maven -> Repositories -> 选中本地仓库 -> 点击 Update

