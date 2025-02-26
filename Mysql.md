<!-- when comment system will be scalable from practice side then we will display  Article/Discussion tab-->

# MySQL Interview Questions

****MySQL ****is a Free open-source ****Relational Database Management System(RDMS)**** that stores data in a structured tabular format using rows and columns. It uses Structured Query Language (SQL) for accessing, managing, and manipulating databases. It was originally developed by MySQL AB, a Swedish company, and is now owned by Oracle Corporation. It’s known for its high performance, reliability, and ease of use, making it one of the most popular databases in the world.

Here, we’ll cover ****50+ MySQL Interview Questions with answers ****that are asked in Data Analyst/SQL Developer Interviews at MAANG and other high-paying companies. Whether you are a ****fresher ****or an ****experienced professional**** with 1, 5, or 10+ years of experience, this article gives you all the confidence you need to ace your next interview.

Table of Content

* [MySQL Interview Questions And Answers for Freshers](#basics-mysql-interview-questions)
* [Intermediate MySQL Interview Questions and Answers](#intermediate-mysql-interview-questions)
* [Advanced MySQL Interview Questions For Experienced](#advanced-mysql-interview-questions)

## MySQL Interview Questions And Answers for Freshers

### 1. What is MySQL and How does it differ from other relational databases?

MySQL is an ****open-source**** relational database management system (****RDBMS****) that is widely used for ****managing structured data****. It utilizes SQL (Structured Query Language) for ****querying**** and ****managing data****. MySQL is known for its reliability, scalability, and performance, making it a popular choice for various applications

### 2. How to create a database in MySQL?

To create a database in MySQL, we can use the ****CREATE DATABASE**** statement followed by the name we want to give to our database. For example:

```
CREATE DATABASE mydatabase;
```

### 3. Difference between CHAR and VARCHAR data types.

* ****CHAR: ****Fixed-length character data type where the storage size is predefined. Trailing spaces are padded to reach the defined length.
* ****VARCHAR:**** Variable-length character data type where the storage size depends on the actual data length. No padding of spaces is done.

### 4. Explain the differences between SQL and MySQL?

| SQL                                                                                                   | MySQL                                                                                             |
| ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| It is a structured query language that manages the relational database management system.             | It is a relational database management system that uses SQL.                                      |
| It is not an open-source language.                                                                    | MySQL is an open-source platform. It allows access to anyone.                                     |
| SQL supports [XML](https://www.geeksforgeeks.org/xml-basics) and user defined functions.              | It doesn’t support XML and any user defined functions                                             |
| SQL can be implemented in various RDBMS such as PostgreSQL, SQLite, Microsoft SQL Server, and others. | MySQL is a specific implementation of an RDBMS that uses SQL for querying and managing databases. |
| SQL itself is not a product and doesn’t have a license. It’s a standard language.                     | MySQL is open-source and available under the GNU General Public License (GPL).                    |

### 5. What is the MySQL server’s default port?

****3306**** is [MySQL server](https://www.geeksforgeeks.org/how-to-stop-mysql-server-on-windows-and-linux)‘s default port.

### 6. How can we learn batch mode in MySQL?

Below is the syntax used to run [batch](https://www.geeksforgeeks.org/batch-command-in-linux-with-examples) mode.

> mysql \<batch-file>;
>
> mysq \<batch-file> mysql.out

### 7. How many different tables are present in MySQL?

There are**** 5 types of tables ****present in MySQL.

* [Heap](https://www.geeksforgeeks.org/heap-sort) table
* [merge](https://www.geeksforgeeks.org/merge-sort) table
* MyISAM table
* INNO DB table
* ISAM table

### 8. What are**** the differences between CHAR and VARCHAR data types in MySQL?****

* Storage and retrieval have been different for CHAR and VARCHAR.
* Column length is fixed in CHAR but VARCHAR length is variable.
* CHAR is faster than VARCHAR.
* CHAR datatype can hold a maximum of 255 characters while VARCHAR can store up to 4000 characters.

### 9. What is ****Difference between CHAR\_LENGTH and LENGTH?****

[LENGTH](https://www.geeksforgeeks.org/length-function-in-mysql) is byte count whereas [CHAR\_LENGTH](https://www.geeksforgeeks.org/char_length-function-in-mysql) is character count. The numbers are the same for Latin characters but different for Unicode and other encodings.

****Syntax of CHAR\_LENGTH:****

> SELECT CHAR\_LENGTH(column\_name) FROM table\_name;

****Syntax of LENGTH:****

> SELECT LENGTH(column\_name) FROM table\_name;

### 10. What do you understand by % and \_ in the like statement?

****‘\_’ ****corresponds to only one character but ‘%’ corresponds to zero or more characters in the [LIKE](https://www.geeksforgeeks.org/sql-like) statement.

### 11. How many index columns can be created in a table?

There are ****16**** indexed columns can be created in a table.

### 12. What are string types available for columns?

There are six string types available for the column.

* [SET](https://www.geeksforgeeks.org/sets-in-javascript)
* [BLOB](https://www.geeksforgeeks.org/blob-full-form)
* TEXT
* [ENUM](https://www.geeksforgeeks.org/enumeration-enum-c)
* CHAR
* VARCHAR

### 13. Explain the main difference between FLOAT and DOUBLE?

* [FLOAT](https://www.geeksforgeeks.org/css-float) stored floating point number with 8 place accuracy. The size of FLOAT is 4 bytes.
* [DOUBLE](https://www.geeksforgeeks.org/difference-float-double-c-cpp) also stored floating point numbers with 18 place accuracy. The size of DOUBLE is 8 bytes.

### 14. Explain the differences between BLOB and TEXT.

****BLOB:****

A [BLOB](https://www.geeksforgeeks.org/retrieve-image-and-file-stored-as-a-blob-from-mysql-table-using-python) is a large object in binary form that can hold a variable amount of data. Sorting and comparing in BLOB values are case-sensitive.

There are four types of BLOB.

* TINYBLOB
* BLOB
* MEDIUMBLOB
* LONGBLOB

****TEXT:****

[Sorting](https://www.geeksforgeeks.org/sorting-algorithms) and comparison are performed in case-insensitive for TEXT values. we can also say a TEXT is case-insensitive BLOB.

There are four types of TEXT.

* TINYTEXT
* TEXT
* MEDIUMTEXT
* LONGTEXT

### 15. Explain the ****difference between having and where clause in MySQL.****

* [WHERE](https://www.geeksforgeeks.org/sql-where-clause) statement is used to filter rows but [HAVING](https://www.geeksforgeeks.org/sql-having-clause-with-examples) statement is used to filter groups.
* [GROUP BY](https://www.geeksforgeeks.org/sql-group-by) is not used with WHERE. HAVING clause is used with GROUP BY.

### 16. Explain REGEXP?

[REGEXP](https://www.geeksforgeeks.org/mysql-regular-expressions-regexp) is a pattern match where the pattern is matched anywhere in the search value.

For more detail you refer to our [MySQL | Regular expressions](https://www.geeksforgeeks.org/mysql-regular-expressions-regexp) Article.

### 17. How can we add a column in MySQL?

A ****column**** is a series of table cells that store a value for table’s each row. we can add column by using [ALTER TABLE ](https://www.geeksforgeeks.org/sql-alter-add-drop-modify)statement.

> ALTER TABLE tab\_name
>
> ADD COLUMN col\_name col\_definition \[FIRST|AFTER exist\_col];

### 18. How to delete columns in MySQL?

We can remove columns in MySQL by using [ALTER TABLE](https://www.geeksforgeeks.org/sql-alter-rename) statement.

****Syntax:****

> ****ALTER**** ****TABLE**** table\_name ****DROP**** ****COLUMN**** column1, column2….;   

### 19. How to delete a table in MySQL?

We can delete a table by using [DROP TABLE](https://www.geeksforgeeks.org/hive-drop-table) statement. This statement deletes complete data of table.

> DROP TABLE table-name;

### 20. How are mysql\_fetch\_array() and mysql\_fetch\_object() different from each another?

mysql\_fetch\_array() Gets a result row as a related array or a regular [array](https://www.geeksforgeeks.org/array-data-structure) from database. mysql\_fetch\_object gets a result row as an [object](https://www.geeksforgeeks.org/object-class-in-java) from the database.

### 21. How to get the top 10 rows?

The following query will be used to get top 10 rows.

> SELECT \* FROM table\_name LIMIT 0,10;

### 22. How does NOW() differ from CURRENT\_DATE()?

current year, month, and date with hours, minutes, and seconds is shown by using [NOW()](https://www.geeksforgeeks.org/now-function-in-mysql) command while [CURRENT\_DATE](https://www.geeksforgeeks.org/current_date-function-in-mysql) shows current year current month, and current date.

****Syntax:****

> SELECT NOW();
>
> SELECT CURRENT\_DATE();

### 23. ****What is the use of the ‘DISTINCT’ keyword in MySQL?****

the [DISTINCT](https://www.geeksforgeeks.org/postgresql-distinct-on-expression) keyword allows for the removal of all duplicate records and the retrieval of unique records.**** The ****DISTINCT keyword is used with the SELECT statement.

****Syntax:****

> SELECT DISTINCT colu1, colum2..
>
> FROM table\_name;

### 24. Which storage engines are used in MySQL?
InnoDB
MyISAM
Memory
CSV

### 25. How to create a table in MySQL?

The [CREAT TABLE](https://www.geeksforgeeks.org/postgresql-create-table) command will be used to create a table in MySQL.

****Syntax:****

> CREATE TABLE ‘Employee’ (‘Employee\_Name’ VARCHAR(128), ‘Employee\_ID’ VARCHAR(128), ‘Employee\_Salary’ VARCHAR(16), ‘Designation’ CHAR(4)) ;

### 26. How to insert data in MySQL table?

We can add data to a table using the [INSERT INTO](https://www.geeksforgeeks.org/sql-insert-statement) statement .

****Syntax:****

> ****INSERT**** ****INTO**** table\_name ( field1, field2, field3 )  
>
> ****VALUES****  ( value1, value2, value3 );  

## Intermediate MySQL Interview Questions and Answers

### 27. ****Write a statement to find duplicate rows In the MySQL table?****

The below statement is used to find duplicate rows.

> SELECT Table\_Name, Category
>
> FROM Product
>
> GROUP BY Name, Category
>
> HAVING COUNT(id) > 1;

### 28. What types of relationships are used in MySQL?

There are three types of [relationships](https://www.geeksforgeeks.org/recursive-relationships-in-er-diagrams) used in MySQL.

****One-to-one:**** Elements with a [one to one](https://www.geeksforgeeks.org/hibernate-one-to-one-mapping) relationship can be included as columns in the table.

****One-to-many:**** One to many or many to one relationships both are same. It will occur when one row in a table is related to multiple rows in different table.

****Many-to-many: ****Many rows in a table are related to many rows in different table is called many to many relationship.

### 29. How to insert Date in MySQL?

We can use INSERT statement to insert date in MySQL table. MySQL default date format is YYYY-MM-DD. Automatic MySQL consist many data types to store dates.

* DATE
* DATETIME
* TIMESTAMP
* YEAR

****Syntax:****

> ****INSERT**** ****INTO**** table\_name (column\_name, column\_date) ****VALUES**** (‘DATE: Manual Date’, ‘2023-5-20’);   

### 30. What is join? Tell different join in MySQL.

[Joins](https://www.geeksforgeeks.org/sql-join-set-1-inner-left-right-and-full-joins) are used to connect two or more tables. It returns only same values in all tables.

There are four different ways to join MySQL tables.

* Inner Join
* left Join
* Right Join
* Full Join

### 31. What is a primary key? How to drop the primary key in MySQL?

A primary key in MySQL is a single field or a group of fields that are used to uniquely identify each record in a table. A primary key cannot be null or empty. [ALTER TABLE](https://www.geeksforgeeks.org/sql-alter-add-drop-modify) statement is used to delete a primary key from a table.

****Syntax:****

> ****ALTER**** ****TABLE**** table\_name  ****DROP**** ****PRIMARY**** ****KEY****;    

### 32. What is a heap table in MySQL?

A [heap](https://www.geeksforgeeks.org/heap-data-structure) table is usually used for temporary and fast temporary storage.

* BLOB or TEXT fields are not permitted in the heap table.
* [comparison operator](https://www.geeksforgeeks.org/javascript-comparison-operators) like =, <,>, = >,=< can be used only.
* Heap table didn’t support the AUTO\_INCREMENT command.
* Indexes should be NOT NULL in the heap table.

### 33. What is the main difference between the primary key and the candidate key?

The primary key uniquely identified each row of a table. only one primary key is available for a table.

* A primary is also a [candidate key](https://www.geeksforgeeks.org/difference-between-primary-and-candidate-key).
* Candidate key that can be used for all [foreign key](https://www.geeksforgeeks.org/postgresql-foreign-key) references.

For mor detail you can see: [Difference between Primary and Candidate Key](https://www.geeksforgeeks.org/difference-between-primary-and-candidate-key)

### 34. ****What is the difference between DELETE and TRUNCATE commands in MySQL?****

[****DELETE****](https://www.geeksforgeeks.org/sql-delete-statement)**** ****Command is used to delete rows from the table depending on given the condition. [TRUNCATE](https://www.geeksforgeeks.org/sql-drop-truncate) command is used to DELETE all rows from the table. DELETE command is a Data Manipulation Language command. TRUNCATE command is a Data Definition Language command.

For More detail you can see : [Difference between DELETE and TRUNCATE](https://www.geeksforgeeks.org/difference-between-delete-and-truncate)

### 35. What is InnoDB?

A SQL storage database is called InnoDB database. The InnoDB offers [ACID transactions](https://www.geeksforgeeks.org/acid-properties-in-dbms), row-level locking, and foreign key support. InnoDB is owned by Oracle Corporation.

### 36. ****What is the difference between UNION and UNION ALL in MySQL?****

During combining the results of more than one SELECT statement, the [UNION](https://www.geeksforgeeks.org/union-and-union-all-in-ms-sql-server) operator deletes duplicate rows between the various SELECT statements. The [UNION ALL](https://www.geeksforgeeks.org/union-union_all-functions-in-dplyr-package-in-r) also combines the result set of more than one SELECT statement, but it does not delete duplicate rows.

### ****37. What is a ‘timestamp’ in MySQL?****

In MySQL, When a row is added to or updated in a table, a data type “[timestamp](https://www.geeksforgeeks.org/get-current-timestamp-using-python)” automatically records the time.

### 38. What is the use of ENUMs in MySQL?

ENUM is a string [object](https://www.geeksforgeeks.org/objects-in-javascript) that can be used when creating tables to specify a set of predefined values.

> CREATE table size(name ENUM(‘Small’, ‘Medium’, ‘Large’);

For more detail refer to those article on [Enumerator (Enum) in MySQL](https://www.geeksforgeeks.org/enumerator-enum-in-mysql)

### 39. How can you control max size of heap in MySQL?

MySQL config variable **max\_heap\_table\_size** can be used to control the max size of [heap](https://www.geeksforgeeks.org/heap-sort).

****Syntax:****

> SET max\_heap\_table\_size = M

### 40. What is a view? How to create a view?

A database object that has no value is called view. Rows and columns exist in a view. A view is virtual table. it is created by combining one or more tables. The difference of a view and a table is that views are definition that build on other tables. If the underlying table changes, the View will also reflect those same changes.

The below syntax is used to create a view.

****Syntax:****

> ****CREATE**** ****VIEW**** view\_name ****AS****    
>
> ****SELECT**** columns    
>
> ****FROM**** tables    
>
> \[****WHERE**** conditions];    

### 41. Where MyISAM table will be stored and also give MyISAM formats of storage?

Every MyISAM table is stored on [disk](https://www.geeksforgeeks.org/c-look-disk-scheduling-algorithm). 

There are three storage formats can be used .

* The .frm file can be used to store table definition.
* The .MYD( MYData) extension can be used for data files.
* The .MYI(MYIndex) extension can be used to Index files.

### 42. How can we save images in MySQL?

In MySQL, Blobs can be used to store images. All [database images](https://www.geeksforgeeks.org/how-to-upload-image-into-database-and-display-it-using-php) are first converted into blobs then saved and then they will be added to the database, and finally, it will later be stored on the disk.

### 43. What are trigger and how many TRIGGERS are available in MySQL table?

A [trigger](https://www.geeksforgeeks.org/sql-trigger-student-database) is a procedural code in a database. Triggers are automatically triggered when specific events occur on a particular table. During column updating triggers are invoked automatically.

SIX triggers are available in MySQL table.

* BEFORE INSERT
* AFTER INSERT
* BEFORE UPDATE
* AFTER UPDATE
* BEFORE DELETE
* AFTER DELETE

For more detail you can see: [Different types of MySQL Triggers (with examples) – GeeksforGeeks](https://www.geeksforgeeks.org/different-types-of-mysql-triggers-with-examples)

### 44. What are the different characteristics of MySQL MyISAM Static and MyISAM Dynamic?

* Width of all fields is fixed in MyISAM [Static](https://www.geeksforgeeks.org/static-keyword-cpp) table whereas width of all fields is not fixed in MyISAM [Dynamic](https://www.geeksforgeeks.org/dynamic-programming). In MyISAM Dynamic table width will be like TEXT, BOLD, etc.
* In case of corruption MyISAM static table is easy to store.

## MySQL Interview Questions For Experienced

### 45. What are Access Control Lists?

A list of permissions known as an [Access Control List](https://www.geeksforgeeks.org/access-lists-acl) is connected to an object. It is MySQL server security model helps in troubleshooting issues like users being unable to connect. MySQL holds the ACL’s cached in memory. ACL’s also called grant tables. MySQL verifies the authentication data and permissions against the ACLs. It predetermined order whenever a user tries to log in or execute a command.

### ****46. What is Normalization and list the different types of normalization?****

[****Normalization****](https://www.geeksforgeeks.org/introduction-of-database-normalization) is used to avoid duplication and redundancy. it is a process of organizing data. There are many normal forms of normalization. which are also called successive levels. The first three regular forms are sufficient.

* ****First Normal Form (1NF):**** There are no repeating groups within rows.
* ****Second Normal form(2NF):**** Value of every supporting column depending on the whole primary key.
* ****Third Normal Form(3NF): ****It depends only on the **primary key** and no other value of non-key column.

### 47. W****hat are various ways to create an index?****

There are many options to create an index as below:

* [T-SQL](https://www.geeksforgeeks.org/difference-between-t-sql-and-pl-sql) statements can be used to create an index.
* The SQL Server Management Studio is available for use. we can use this to browse to the table where the index will be created, and then right-click on the Indexes node. We must select the New Index option over here.
* We can identify the index indirectly by specifying the [PRIMARY KEY](https://www.geeksforgeeks.org/difference-between-primary-key-and-unique-key) and the [UNIQUE](https://www.geeksforgeeks.org/postgresql-unique-index) constraint in the [CREATE TABLE](https://www.geeksforgeeks.org/python-sqlite-create-table) or [ALTER TABLE](https://www.geeksforgeeks.org/sql-alter-add-drop-modify) statement.

### 48. What are a clustered index and a non clustered index(secondary index)?

****Cluster Index:**** An index type used to arrange data in a table is called a [clustered index](https://www.geeksforgeeks.org/clustering-indexing-in-databases). The table’s data are stored in a specific order based on the clustered index.

****Non Cluster Index:**** A [non-clustered index](https://www.geeksforgeeks.org/sql-queries-on-clustered-and-non-clustered-indexes) is also a type of index used to organize data in a table. The table’s data are not stored in a specific order based on the non clustered index.

For more details, Check our latest article on [Difference between Clustered and Non-clustered index](https://www.geeksforgeeks.org/difference-between-clustered-and-non-clustered-index).
聚簇索引（Clustered Index）	叶子节点存储完整的数据行
二级索引（Secondary Index）	叶子节点存储主键 ID，而不是完整数据
使用聚簇索引（主键索引）查询时，不需要回表，因为叶子节点就包含了完整的数据行。
使用二级索引时，如果查询列不包含在索引中，就需要回表查询完整数据（即 回表（Back to Clustered Index））。

### 49. How to**** validate emails using a single query?****

We can use the [regular expressions function](https://www.geeksforgeeks.org/regular-expressions-in-c) (REGEXP\_LIKE) to validate emails. Below is the example of validate emails using a single query.

> ****SELECT****
>
> Email
>
> ****FROM****
>
> Vehicle
>
> ****where**** NOT REGEXP\_LIKE(Email, ‘\[A-Z0-9.\_%+-]+@\[A-Z0-9.-]+.\[A-Z]{2,4}’, ‘i’);

For detail you can check our latest article on [Regular expressions (Regexp)](https://www.geeksforgeeks.org/mysql-regular-expressions-regexp).

### 50. ****How can you handle the –secure-file-****priv**** in MySQL?****

The MySQL Server is restricted from loading directories using the [LOAD DATA INFILE](https://www.geeksforgeeks.org/how-to-import-timestamp-from-a-csv-file-in-mysql) command by the -secure-file-priv option. Use the SHOW VARIABLES LIKE “secure\_file\_priv” command to view the directory that has been configured.

There are two options to handle as below.

* Either transfer your file to the directory that secure-file-priv specifies.
* Or you can turn off secure-file-priv. This must be removed at the beginning and cannot be disabled later.

### 51. ****Whats the difference between NULL and ''****
1. When querying NULL values, you must use IS NULL or IS NOT NULL to determine their presence, as comparison operators such as =, !=, <, and > cannot be used. However, '' (empty string) can be used with these comparison operators.
2. ''的长度是 0，是不占用空间的，而NULL 是需要占用空间的。

### 52. ****The execution flow of a SQL statement in MySQL''****
1. **Connection Manager** -> verifies the client’s authentication and checks if the user has the necessary privileges to execute the query.
2. **Parser** -> The query is sent to the Parser, where MySQL verifies the syntax to ensure it is correctly formatted.
3. **Query Optimizer**-> The Query Optimizer takes the parse tree and determines the most efficient execution plan
4. **Executor** -> The Executor executes the query using the selected plan, interacting with the Storage Engine
### 53. ****MyISAM vs InnoDB''****
1. 事务 Transaction
2. 行级锁 row-level locking
3. 外键 foreign key
4. 崩溃后安全恢复
5. MVCC
6. 索引实现不一样
7. 性能有差异
8. innoDB使用buffer pool缓存数据页以及索引页面, MyIsAM用Key Cache缓存索引页不缓存数据页

### 54.How to deal with huge tables?
1.  水平分表: Horizontal Partitioning-> Split a large table into smaller tables based on a key
2.  垂直分表: Vertical Partitioning-> Split a wide table into multiple smaller tables by moving less frequently used columns into separate tables.
3.  索引优化: index optimization-> Use covering indexes,Avoid too many indexes
4.  读写分离: read & write split
5.  分析查询: EXPLAIN -> Use EXPLAIN ANALYZE to find slow queries.

### 55. Query time analyze?
>启用SET profiling = 1;
>运行SQL
>查询总的运行时间SHOW PROFILES;
>查看SQL执行各个阶段的耗时 SHOW PROFILE FOR QUERY 1;
Opening tables-> too much join operation
System lock	-> 
Optimizing -> wrong index
Statistics -> table data too large
Sending data-> table data too large
使用 EXPLAIN / EXPLAIN ANALYZE (select_type, type, key, extra) -> judge whether the index is being used correctly.
type = ALL → 说明是 全表扫描，应考虑增加索引
rows = 1000000 → 说明扫描的行数过多，可能需要 优化 WHERE 条件
key(实际使用的索引) = NULL → 说明没有使用索引，需要 增加索引

### 56. Covering Index? & Composite Index?
> A Covering Index is an index that contains all the columns needed for a query, so the database engine can retrieve the required results directly from the index without accessing the actual table data. This improves query performance by reducing I/O operations.
> 由多个列组成的索引，提高组合查询效率,适用于 WHERE 子句有多个字段的组合查询

### 57. Mysql 备份方案?
1. mysqldump/mysqlpump备份 export sql
2. Percona XtraBackup

### 58.Mysql 三大日志?
**redo log**（重做日志）是 InnoDB 存储引擎独有的，它让 MySQL 拥有了崩溃恢复能力。比如 MySQL 实例挂了或宕机了，重启时，InnoDB 存储引擎会使用 redo log 恢复数据，保证数据的持久性与完整性。
**binlog** 可以说 MySQL 数据库的数据备份、主备、主主、主从都离不开 binlog，需要依靠 binlog 来同步数据，保证数据一致性。记录内容是语句的原始逻辑。
**undo log** 属于逻辑日志，记录的是 SQL 语句，比如说事务执行一条 DELETE 语句，那 undo log 就会记录一条相对应的 INSERT 语句。

### 59.最左匹配原则（Leftmost Prefix Matching Rule）
>在使用联合索引进行查询的时候，如果不遵循「最左匹配原则」，联合索引会失效，这样就无法利用到索引快速查询的特性了。
比如，如果创建了一个 (a, b, c) 联合索引，如果查询条件是以下这几种，就可以利用联合索引：
where a=1；
where a=1 and b=2 and c=3；
where a=1 and b=2；
需要注意的是，因为有查询优化器，所以 a 字段在 where 子句的顺序并不重要。但是，如果查询条件是以下这几种，因为不符合最左匹配原则，所以就无法匹配上联合索引，联合索引就会失效:
where b=2；
where c=3；
where b=2 and c=3；
上面这些查询条件之所以会失效，是因为(a, b, c) 联合索引，是先按 a 排序，在 a 相同的情况再按 b 排序，在 b 相同的情况再按 c 排序。所以，b 和 c 是全局无序，局部相对有序的，这样在没有遵循最左匹配原则的情况下，是无法利用到索引的。

### 60.查询缓存（Query Cache) V.S缓冲池（Buffer Pool）
缓存内容	SQL 查询结果	数据页、索引页

### 61.Mysql锁， select 会加锁吗？什么情况下会加锁？
默认情况下，普通的 SELECT 语句不会加锁，只是执行 MVCC（多版本并发控制） 机制，以**快照读Snapshot Read**方式读取数据，不阻塞其它事务的更新。

### 62.sql injection?
parameter concatenation
传参数方式解决SQL注入

### 63. MyISAM 与 InnoDB 区别：
InnoDB支持事务 
InnoDB支持外键
InnoDB支持row-level lock
InnoDB支持崩溃后恢复, 基于redo log
InnoDB支持MVCC

