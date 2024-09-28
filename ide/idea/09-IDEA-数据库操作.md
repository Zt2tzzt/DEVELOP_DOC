# IDEA 数据库操作

在 IDEA 右侧面板中，集成了数据库图形化工具。

使用该工具，连接数据库前，要先下载对应数据库的驱动，比如 MySQL 的驱动。

## 一、查询控制台

右键数据库连接 -> Navigation -> Jump to Query Console；跳转到之前使用过的查询控制台。

## 二、查看表结构关联关系

在 IDEA 中，选中有关联关系的表，右键 -> Show Diagram

## 三、IDEA 配置 MyBatis SQL 提示

在 `xxxMapper` 接口中，使用注解的方式编写 SQL 可进行如下操作：

- 右键注解（比如：`@Select`）中的 SQL 语句 -> 点击 “Show Context Actions” -> 点击 “Language Injection Setting” -> ID 选择 MySQL；
