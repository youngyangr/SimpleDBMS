# DBMS.......一个用Java实现的关系型数据库

### 实现功能
* 1、用Java语言建立数据库表。  
（1） 数据文件和字典文件存储结构和存取方法为按行存取，数据为字符型可直接阅读。  
（2） 属性的个数任意，属性的类型包括整数int,字符串varchar,双精度浮点double。  
（3） 表的相关信息存入数据字典。  

* 2、为关系表插入元组。  
（1） 用VALUES子句为新建立的关系插入元组。  
（2） 用VALUES子句在关系模式修改之后按照新的模式插入元组。  
（3） 不指定属性，插入元组的所有属性值；  
（4） 插入元组的指定属性的值。  
（5） 修改相应的索引文件。  

* 3、实现属性的添加和删除功能。  
（1）为基本表添加属性并维护数据字典。  

* 4、实现表中元组的删除和修改功能，维护索引文件。  
（1）实现删除数据库记录的功能。  
    a) 没有WHERE条件，删除关系中的所有元组。  
    b) 指定WHERE条件，删除满足条件的元组。  
（2）实现修改数据库记录的功能。  
    a) 没有WHERE条件，修改所有元组的指定属性的值。  
    b) 指定WHERE条件，修改满足条件的元组的指定属性的值。  
（3）修改相应的索引文件。  

* 5、实现表的删除功能。  
（1）删除表并维护数据字典。  
（2）删除相应的索引文件。  

* 6、索引的创建、维护与删除  
（1）为关系表的所有属性建立稠密索引(文件路径+文件行号)。  
（2）使用java类库的treeMap(红黑树实现)存储索引项。  
（3）实现数据增删改时索引的维护功能。  
（4）实现数据增删改查时，从索引树中索引所需的数据文件，提高数据操作效率。  
（5）可控制文件行数，默认：lineNumConfine = 10;每插满10行，新建数据文件。  

* 7、实现显示数据库表的功能。  
（1）实现“SELECT * FROM 表名”。  
（2）显示表的结构和内容。  

* 8、查询优化：  
(1)实现启发式关系代数优化算法。（对原始的语法树进行优化处理，生成查询计划，选择代价最小的。）  

* 9、查询执行：  
 (1)、实现单关系的投影操作（select 属性名列表 from 关系名）。  
 (2)、实现单关系的选择操作（select * from 关系名 where 条件表达式）。  
 (3)、实现单关系的选择和投影操作（select 属性名列表 from 关系名 where 选择条件）。//选择条件是指“属性名 操作符 常量”形式的条件  
 (4)、实现多个关系的选择、投影和连接操作（select 属性名列表 from 关系名列表 where 条件表达式）。  
 (5)、实现两个关系和多个关系的连接操作（select * from 关系名列表 where 连接条件）。//连接条件是指“属性名 操作符 属性名”形式的条件  
 (6)、实现多个关系的选择、投影和连接操作（select 属性名列表 from 关系名列表 where 条件表达式）。  

* 10、用户权限  
（1）、创建用户、设置密码，并写数据字典；  
（2）、为用户授权，并写数据字典(grant admin to userName;)；  
（3）、用户进行任何数据库操作前，要根据数据字典进行权限验证；  
（4）、撤销用户权限，并修改数据字典(revoke admin from userName;)。  

# SimpleDBMS
