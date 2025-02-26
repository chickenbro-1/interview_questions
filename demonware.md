DB: sharding, replication, how to deal with Huge tables. Query time analyze. 
Redis, data types, sharding replica.
Python db pool libs
Networks: troubleshooting, Linux commands: netstat, telnet, lsof .....
OSI models.
docker containerize
kubernetes


### 1. 索引策略以及sql查询优化
1. **慢SQL定位与分析**
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

2. **索引创建原则**

不为null字段加索引
给频繁查询的字段加索引
给作为查询条件的字段加索引, where之后的条件
给频繁排序的字段加索引
索引一张表不应该超过5个

覆盖索引(Covering Index)
索引中已经包含了所有需要获取的字段的查询方式称为覆盖索引。避免 InnoDB 表进行索引的二次查询(避免使用回表)

3. **SQL优化:**
避免使用select all the columns in the table
使用连接查询代替子查询(避免 `IN`，使用 `EXISTS` 或 `JOIN`)Use JOIN queries instead of subqueries.


4. **数据库参数调优:**

调整 `innodb_buffer_pool_size` index and data page, the half of the physical memory

5. **增加缓存机制**
使用Redis加一个缓存层

![alt text](image-2.png)
### 2.重新设计restfui api

防止返回过多的**data**
(避免**嵌套查询**)避免 **N+1 查询**，减少不必要的 API 调用
**逻辑修改**: 批量上传图片改为用户点击一次上传一次

### 3.python数据库连接池(database connection pool)

sqlalchemy
QueuePool（默认池）
在 SQLAlchemy 中，数据库连接池的配置主要通过 create_engine() 的参数进行控制

### 4.redis message queue?

- **订单生成**：订单对象存入 Redis(hset)，并初始状态设为“待支付”。
- **支付回调**：
    - 支付 API 异步返回结果后，读取订单对象(hgetall),更新订单状态为“支付成功”或“支付失败”。
    - 如果支付成功，使用 XADD 将支付成功的消息写入 Stream。
- **开卡服务**：
    - 通过消费者组监听 Stream 消息，收到支付成功消息后调用开卡 API。使用xrange()读取消息,xread() 或 xreadgroup()消费数据.
    - 开卡成功后更新订单状态，并使用 XACK 确认消息处理完毕。