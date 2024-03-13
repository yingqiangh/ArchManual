# 任务调度（分布式定时任务）
## 场景

任务调度是指系统在约定的特定时刻自动去执行指定任务的过程。
比如：
- 某新闻App每天上午10点给用户推送最新新闻。
- 某电商系统需要在每天上午 10 点，下午 3 点，晚上 8 点等不同适合发放一批优惠券。
- 某银行系统需要在信用卡到期还款日的前三天每天进行短信提醒。
- 某财务系统需要在每天凌晨 1点 结算前一天的财务数据，统计汇总。
- 某报表系统需要在每天凌晨 1点 读取业务数据生成报表数据。
- 12306 会根据车次的不同，而设置某几个时间点进行分批放票。

## 功能
一个任务调度平台，需要具备有以下几点功能：
- **核心功能**：定时调度、任务管理、日志监控
- **高可用**：集群、分片、失败处理
- **高性能**：分布式锁
- **扩展功能**：可视化运维、多语言、任务编排 
 
## 架构
### 1. 如何调度
### 2. 如何分片 

## 工具
推荐

- [xxl-job](https://github.com/xuxueli/xxl-job)
- [Elastic-job](https://github.com/apache/shardingsphere-elasticjob)
- [powerJob](https://github.com/PowerJob/PowerJob)

其他

- [Saturn](https://github.com/vipshop/Saturn)
- [Quartz](https://github.com/quartz-scheduler/quartz)
