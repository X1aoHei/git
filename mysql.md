## 分表分区

* mysql的数据主要存储到/mysql/data下面。一个表对应三个文件，一个是frm保存表结构，一个是myd存放表数据，一个是myi存放表索引

## mysql锁机制

### 行锁

* 锁的类型：共享锁（S LOCK）和排它锁（X LOCK）。允许事务读一行数据
* ![1564381938268](C:\Users\WSS\AppData\Roaming\Typora\typora-user-images\1564381938268.png)

### 表锁（意向锁）

* 意向共享锁（IS LOCK）事务想要获取一张表里面的某几行的共享锁
* 意向排它锁（IX LOCK）事务想要获取一张表里面的某几行的排它锁
* ![1564382311010](C:\Users\WSS\AppData\Roaming\Typora\typora-user-images\1564382311010.png)

* 