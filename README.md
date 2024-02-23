# ArchManual

### 项目介绍
ArchManual  
**不是**：   
某个技术架构的深度剖析  
某个技术框架的源码分析  
某个技术工具的安装运维   
某个技术类库的代码示例   
**而是**：  
常用分布式技术的总体概览  
常用技术主题的归纳总结  
常用技术框架的归类罗列  
常用技术架构的简单分享  
**希望成为**：  
速查手册：平时工作中做技术架构、框架选型时的速查手册    
学习提纲：业余学习或者面试时的一个学习提纲   
技术地图：希望能起到一些指引的作用。也希望每个技术小伙伴都能积极参与，分享知识，丰富`ArchManual`

### 整体概览 
- 概览图：  
![整体概览](overview/ArchManual.jpg)  
- 地址：  
[思维导图](https://www.processon.com/view/link/65b74ca5ec61176de3760fc3)

### 导航

- [后端主题](#后端主题)
- [前端主题](#前端主题)
- [系统运维](#系统运维)
- [监控](#监控)
- [大数据](#大数据)
- [系统安全](#系统安全)
- [通用架构](#通用架构)
- [人工智能](#人工智能)  

#### 后端主题
- [配置中心](config/index.md)  
    - [Apollo](https://github.com/apolloconfig/apollo)
    - [Nacos](https://github.com/alibaba/nacos)
    - [Spring Config](https://github.com/spring-cloud/spring-cloud-config)
    - [Disconf](https://github.com/knightliao/disconf)
- [消息队列](mq/index.md)
    - 分布式消息队列
        - [Kafka](https://github.com/apache/kafka)
        - [RocketMQ](https://github.com/RocketMQ)
        - [RabbitMQ](https://github.com/rabbitmq)
        - [ActiveMQ](https://github.com/apache/activemq)
        - [Redis](https://github.com/redis/redis)
    - 内存消息队列（线程间消息传递）
        - [Disruptor](https://github.com/LMAX-Exchange/disruptor)
    - MTTQ（应用于物联网）
        - [EMQX](https://github.com/emqx/emqx)
        - [Mosquitto](https://github.com/eclipse/mosquitto)
        - [NanoMQ](https://github.com/nanomq/nanomq)
- [延迟任务](dq/index.md)
    - 消息队列
        - [RabbitMQ TTL + 死信队列](dq/index.md)
        - [RabbitMQ 延迟队列插件(*推荐)](dq/index.md)
        - [RocketMQ 定时消息(*推荐)](dq/index.md)
    - Redis缓存
        - [定时轮询zset](dq/index.md)
        - [Redis Key过期监听](dq/index.md)
        - [Redisson 分布式延迟队列 RDelayedQueue (*推荐)](dq/index.md)
    - 定时轮询
        - [Spring Task](dq/index.md)
        - [XXL-Job](dq/index.md)
        - [Elastic-Job](dq/index.md)
    - 内存队列
        - [JDK DelayQueue](dq/index.md)
    - 时间轮算法
        - [Netty的HashedWheelTimer](dq/index.md)
        - [Kafka的TimingWheel](dq/index.md)
- 定时任务
- 全局控制
- 注册发现
#### 前端主题
#### 系统运维
#### 监控
#### 大数据
#### 系统安全
#### 通用架构
#### 人工智能
