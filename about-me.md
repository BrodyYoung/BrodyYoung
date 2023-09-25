# 个人信息
- 男 1998.05 统招本科
- Java+JS开发  工作 2年
- 目标城市：北京
- 邮箱：yungyunbo@163.com


# 技术社区
GitHub： https://github.com/BrodyYoung 

CSDN： https://blog.csdn.net/weixin_44816664    

博客园： https://www.cnblogs.com/yunbrody/

掘金： https://juejin.cn/user/34781265158344/posts

# 相关技能

- 熟悉Java语法，熟悉JavaWeb编程，能熟练使用SpringCloud、SpringBoot、MyBatis、SpringSecurity Oauth2、Spring等框架进行web开发，熟悉常用的JAVA设计模式。
- 熟练使用MySQL数据库，熟悉常用SQL语句，能进行SQL索引优化，熟悉Redis、MongoDB、ElasticSearch等NoSQL，熟悉Redis底层原理。
- 熟悉计算机网络知识，熟悉TCP/IP协议，熟悉HTTP协议的编程。
- 熟练使用Netty框架，能使用Netty编写RPC应用，熟悉Dubbo工作原理。
- 熟悉常见的数据结构，熟悉JUC和JVM相关知识，熟练使用JProfiler、Arthas调优工具。
- 熟练使用IDEA、Git、Maven、Postman、Jenkins、Xshell、PowerDesign等开发工具。
- 熟悉分布式、微服务开发思想和工作流程，熟练使用Nginx、Nacos、Redis等中间件。
- 熟练使用Vue框架、Element-ui、HTML、JavaScript、CSS、Nodejs、AJax等前端开发技术。
- 熟练使用Linux、Shell的常见命令，能熟练使用Docker、K8S、Rancher云原生技术。
- 熟悉AMQP和MQTT消息队列协议，熟练使用RabbitMQ、EMQ等消息队列服务。
- 熟练使用python语言，能进行数据爬取分析操作。
- 熟练使用Golang语言，熟练使用Goroutine、Gin、Gorm进行开发。

# 工作经历
2022.10 – 至今             XXX--- 全栈开发工程师

根据需求和原型，负责公司自研的探针设备SaaS平台的Java后台接口开发、前端页面代码编写、与SaaS平台客户数据部门对接、修改bug以及项目中相关文档的撰写。

2020.9 – 2022.10           XXX--- Java开发工程师

根据需求和原型，负责公司自研的能源运营SaaS平台的Java后台接口开发、前端页面和小程序代码编写、与算法和大数据部门对接、修改bug以及项目中相关文档的撰写。

# 项目经历
## XX能源SaaS系统

使用SpringCloud + VUE + Mysql + redis作为主要技术栈

该项目是提供给公司研发人员、商务人员使用的管理后台，为能源SaaS平台提供业务运营和技术运营支撑。有运营平台用户管理和角色管理、资源菜单管理、租户管理、字典管理、系统管理、租户管理后台、项目管理后台等功能模块,可以切换到10多个子系统。

1. 基于Redis + Token机制实现登录验证，解决集群间登录状态同步问题
2. 使用 Redisson 分布式锁来实现操作互斥，防止用户调用接口成功扣减次数后出现剩余次数小于0的问题
3. 选用SpringSecurity作为安全认证框架，基于RBAC实现用户认证、角色管理、资源权限管理
4. 选用SpringCloud Gateway作为API网关，实现路由转发、访问控制，并集中处理签名校验、请求参数校验、接口调用统计等业务逻辑，提高安全性的同时也方便系统开发维护
5. 为解决多个子系统内代码大量重复的问题，抽象模型层和业务层为公共模块，利用Nacos作为注册中心，并使用OpenFeign实现服务间的高性能服务调用，减少重复代码。

## XX设备管理SaaS系统

该项目使用 Springboot + VUE + Mysql + redis 作为主要技术栈。

该项目是为通讯运营商提供的探针设备SaaS管理系统。整个系统包含探针设备管理、定时任务管理、时频误差分析、预警告警反馈等模块，实现管理员对探针设备运行精准管控、对时间频率性能监控的需求。我在该项目担任项目小组长职务，协调前后端开发流程。

1. 基于SNMP网络协议和snmp4j实现Springboot项目与设备通信和数据传输
2. 使用Netty网络编程框架搭建监测服务器，监听SNMP Trap告警信息
3. 基于Nginx实现负载均衡、反向代理、动静分离
4. 使用 Redisson 分布式锁来实现操作互斥，防止用户调用接口成功扣减次数后出现剩余次数小于0的问题
5. 选用SpringSecurity作为安全认证框架，基于RBAC实现用户认证、角色管理、资源权限管理
6. 基于Vue、Element-ui实现前端代码
7. 基于Elasticsearch、Logstash、Kibana实现日志存储分析功能
8. 使用K8s和Rancher对服务进行部署，监测服务运行状况
