# 消息队列
## 场景
- **解耦**：消息队列可以帮助将应用程序的不同组件解耦，使它们可以独立地进行开发、部署和扩展。
- **异步**：消息队列可以用于实现异步处理，提高系统的响应速度和吞吐量。
- **削峰填谷**：消息队列可以用于平滑系统的流量波动。当系统面临突然的高流量时，消息队列可以暂时存储消息，然后由后续的处理者逐渐消费这些消息，防止系统因突发流量而崩溃。
- **日志处理**：消息队列可以用于收集和处理大量的日志数据。应用程序可以将日志信息发送到消息队列，然后由专门的日志处理服务从队列中获取日志并进行分析、存储或展示。
- **任务调度**：消息队列可以用于实现任务调度系统。应用程序可以将需要定时执行的任务信息发送到消息队列，然后由专门的调度器从队列中获取任务并按照预定的时间执行。
- **分布式系统通信**：在分布式系统中，各个节点之间需要进行通信和协调。消息队列可以作为一种分布式通信的基础设施，帮助不同节点之间进行消息交换和数据同步。
- **重试机制**：消息队列可以提供消息重试的机制，当消息处理失败时，可以将消息重新放入队列，等待后续重试，以确保消息被正确处理。
- **事件驱动架构**：消息队列可以用于构建事件驱动架构，通过发布-订阅模式实现系统中的事件通知和处理。

## 功能
- **可靠性**：消息队列应该能够保证消息的可靠传输，即使在系统故障或网络异常的情况下，也能够确保消息不会丢失。为了实现可靠性，通常会采用消息持久化、消息确认机制和消息重试机制等手段。
- **高吞吐量**：消息队列应该能够支持高吞吐量的消息处理，能够处理大量的消息并且保持低延迟。为了实现高吞吐量，需要考虑队列的设计、消息的存储和传输等方面的性能优化。
- **可扩展性**：消息队列应该具备良好的可扩展性，能够根据需求灵活地扩展系统的规模和容量。这包括水平扩展、集群化部署、分区和分片等技术手段。
- **消息排序**：某些场景下，消息的顺序很重要，因此消息队列应该能够保证消息的顺序性。即使是分布式环境下，也需要确保相同分区或主题中的消息能够按照发送顺序进行处理。
- **灵活的消息路由**：消息队列应该支持灵活的消息路由机制，能够根据消息的内容、标签或其他属性将消息路由到不同的队列或主题中，以便于实现定制化的消息处理逻辑。
- **低延迟**：对于一些实时性要求较高的场景，消息队列应该能够保证低延迟的消息传输和处理，尽可能减少消息在队列中的停留时间。
- **可观测性**：消息队列应该提供丰富的监控和管理功能，能够实时监控队列的状态、消息的流动情况、处理速度等指标，并提供相应的报警和日志记录功能，帮助系统管理员进行运维和故障排查。
- **安全性**：消息队列应该具备良好的安全性，能够保护消息的机密性和完整性，防止消息被篡改或者被未授权的访问。这包括数据加密、身份认证、访问控制等安全措施。
- **灵活的部署和集成**：消息队列应该能够与现有的系统和组件进行灵活的集成，支持多种部署方式，包括本地部署、云端部署和容器化部署等。 
 
## 架构
### 1. 高可用 
### 2. 顺序性  
### 3. 消息积压 
### 4. 幂等性 
### 5. 防止丢失  

## 工具
推荐
- Apollo    [官网](https://www.apolloconfig.com/)  [Github](https://github.com/apolloconfig/apollo)  
- Nacos     [官网](https://nacos.io/)  [Github](https://github.com/alibaba/nacos)
- Spring Config [Github](https://github.com/spring-cloud/spring-cloud-config)

其他
- Disconf  [Github](https://github.com/knightliao/disconf)
