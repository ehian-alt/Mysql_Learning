# DML 数据操作

## 添加数据（INSERT）
* 给指定字段添加数据

INSERT INTO 表名 (字段名1，字段名2···) Values (值1，值2···)

* 给全部字段添加数据

INSERT INTO 表名 VALUES (值1，值2···) 

* 批量添加数据

INSERT INTO 表名 (字段名1，字段名2···) Values (值1，值2···),(值1，值2···);
INSERT INTO 表名 VALUES (值1，值2···),(值1，值2···);
## 修改数据（UPDATE）

UPDATE 表名 SET 字段1 = 值1, 字段2 = 值3, ... [WHERE 条件];

## 删除数据（DELETE）

DELETE FROM 表名 [WHERE 条件];

**DELETE语句如果没有条件则会删除整张表的所有数据**
**DELETE 语句不能删除某一个字段的值（可以使用UPDATE）**



