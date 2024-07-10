# Redis
Redis是一种开源的内存数据结构存储，用作数据库、缓存和消息代理。
它支持多种数据结构，如字符串、哈希、列表、集合、有序集合等。

## 应用场景
Redis 在各种应用场景中都有广泛的应用，主要利用其高性能和丰富的数据结构。以下是一些常见的 Redis 应用场景：

### 1. 缓存
**缓存**是 Redis 最常见的应用场景之一。它用于减少数据库的读写压力，加速数据访问，提高系统性能。常用模式包括：

- **旁路缓存（Cache Aside）**：应用程序先查询缓存，未命中则查询数据库，并将结果写入缓存。
- **穿透缓存（Read Through/Write Through）**：所有读写操作都通过缓存，缓存未命中时自动加载数据。
- **回写缓存（Write Behind）**：写操作先写入缓存，再异步写入数据库。

### 2. 会话存储
Redis 非常适合作为会话存储，由于其速度快且支持 TTL，可以存储用户会话数据，并在会话过期后自动删除。

### 3. 实时数据分析
Redis 的数据结构（如计数器、排序集合）使其非常适合用于实时数据分析、计数和排名，如：

- **实时计数**：如网站访问量、点赞数、评论数等。
- **排行榜**：如游戏排行榜、销售排行榜等。

### 4. 消息队列
Redis 支持发布/订阅（Pub/Sub）模式和流（Stream）数据类型，可以用作轻量级的消息队列系统。适用于需要低延迟的消息传递场景。

### 5. 分布式锁
Redis 可以用于实现分布式锁，通过设置带有过期时间的键，确保分布式环境中的资源在同一时刻只被一个客户端占用。Redlock 是一种基于 Redis 的分布式锁实现。

### 6. 数据持久化
Redis 提供 RDB 和 AOF 两种数据持久化机制，可以将内存中的数据持久化到磁盘，防止数据丢失。适用于需要高可用性的应用。

### 7. 地理位置服务
Redis 提供 Geo 数据类型，可以存储和查询地理位置数据，适用于位置服务应用，如查找附近的商店或用户。

### 8. 数据流处理
Redis Streams 数据类型支持高吞吐量的数据流处理，适用于日志收集、实时分析和事件溯源等场景。

### 9. 排序和排名
Redis 的有序集合（Sorted Set）数据类型可以用于实现复杂的排序和排名操作，适用于需要实时更新和查询排名的应用。

### 10. 限流
Redis 的原子操作和高性能使其非常适合用于实现限流和频率控制，如限制 API 请求频率、防止刷单等。

### 11. 计数器
Redis 的原子自增操作非常适合用于实现各种计数器，如访问计数、任务。

## 架构点
Redis的一些常见的架构点如下：
- [数据类型](data.md)
- [过期策略](expire.md)
- [IO模型](io.md)
- [主从复制](master_slave.md)
- [高可用](ha.md)
- [持久化](persistence.md)
- [分布式集群 Redis CLuster](cluster.md)
- [分布式集群 Codis](codis.md)
- [常见问题:雪崩、击穿](problem.md)
- [双写一致性](consistent.md)
- [Key的优化、监测](key.md)

## 工具
- [Redis](https://redis.io/)
- [Redisson](https://github.com/redisson/redisson)
- [Codis](https://github.com/CodisLabs/codis)
- [JD-hotkey](https://gitee.com/jd-platform-opensource/hotkey)
- [Redis Cluster](https://redis.io/docs/latest/operate/oss_and_stack/management/scaling/)
