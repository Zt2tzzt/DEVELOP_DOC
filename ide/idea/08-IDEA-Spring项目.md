# IDEA Spring 项目

## 一、Spring Boot Web 项目创建

1. 进入创建项目窗口：File -> New -> Project；
2. 选择左侧 Spring Boot；
3. 填写右侧信息：
   - Language 设为 Java；
   - Type 设为 Maven；
   - Group 为组织名，比如设为 `com.kkcf`
   - artifact 为项目名，比如设为 `springboot-web-quickstart`；设置完成后，上方 name 会跟着修改。
   - Pacakge name 为要在项目中创建的包的层级，比如设为 `com.kkcf`
   - Java 为 Java 版本；比如设为 17；
   - Pacakging 为打包方式，比如设为 Jar；
4. 点击 Next，进入下一步；
5. 选择 Spring Boot 版本，默认是最新版本。
6. 在下方，勾选 Web -> Spring Web；
7. 点击 Create，联网创建项目；

## 二、Spring Boot Web 结合 MyBatis 项目创建

1. 进入创建项目窗口：File -> New -> Project；
2. 选择左侧 Spring Boot；
3. 填写右侧信息：
   - Language 设为 Java；
   - Type 设为 Maven；
   - Group 为组织名，比如设为 `com.kkcf`
   - artifact 为项目名，比如设为 `springboot-web-quickstart`；设置完成后，上方 name 会跟着修改。
   - Pacakge name 为要在项目中创建的包的层级，比如设为 `com.kkcf`
   - Java 为 Java 版本；比如设为 17；
   - Pacakging 为打包方式，比如设为 Jar；
4. 点击 Next，进入下一步；
5. 选择 Spring Boot 版本，默认是最新版本。
6. 在下方，勾选 Web -> Spring Web；
7. 在下方，勾选 SQL -> MyBatis Framework；勾选 SQL -> MySQL Driver；
8. 点击 Create，联网创建项目；

## 三、MyBatis 配置 MySQL 提示

在 Mabatis 的 Mapper 接口中：

- 右键 @Select 注解中的 SQL 语句 -> 点击 “Show Context Actions” -> 点击 “Language Injection Setting” -> ID 选择 MySQL；

会发现，查询的表 user 报红色。这是因为在 IDEA 中，没有配置操作数据库的连接。所以 IDEA 没法给出 SQL 语句正确性的提示。

- 在 IDEA 右侧 Database 面板中，配置目标数据库的连接即可。
