# 表操作 DDL

* 常见关键词
  * primary key: 主键约束
  * unique: 唯一约束
  * not null: 非空约束
  * default: 默认约束
  * foreign key: 外键约束
  * comment: 字段注释
  * varchar: 可变长度的字符串
  * char(n): 固定长度的字符串
  * data-time: 日期类型
  * tinyint: 小整数值
  * unsigned: 无符号
## 创建表

```sql
create table table_name {
    id int primary key comment 'ID, 唯一标识',
    username varchar(10) comment '用户名',
    age int comment '年龄',
    } comment '示例';
```

## 修改表
* 新增字段

Alter Table 表名 add 字段名 数据类型（长度） comment '';
`alter table table_name add gender char(1) comment '性别';`
* 修改数据类型 

Alter Table 表名 Modify 字段名 新数据类型（长度）
```sql
alter table table_name modify gender tinyint unsigned;
```
* 修改字段名和字段类型

Alter Table 表名 Change 旧字段名 新字段名 类型 comment '';
```sql
alter table table_name change username nickname varchar(20) comment '昵称';
```
* 删除字段

Alter Table 表名 Drop 字段名;
```sql
alter table table_name drop nickname;
```
* 修改表名

Alter table 表名 RENAME 新表名
```sql
alter table table_name rename new_table;
```
* 删除表

```sql
Drop table if exists table_name;    --如果存在table_name 这张表的话就删除
```
```sql
truncate table table_name;      --删除指定表，并重新创建该表
```


