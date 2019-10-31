# Spring Cloud学习笔记

## 觉得整理的不错的朋友，star一下哟，(*￣︶￣)

## 欢迎大家提问题交流

- 项目fork自gongxings/spring-cloud-study，基于自己的理解又添加了修改

![](images/springcloud架构图.png)

## 项目版本

- spring cloud版本：Dalston.SR1
- spring boot版本：1.5.19.RELEASE

## 项目模块说明

``` lua
spring-cloud-study
├── springcloud-study-api -- 构建公共子模块
├── springcloud-study-euraka-7001 -- Eureka集群
├── springcloud-study-euraka-7002 -- Eureka集群
├── springcloud-study-euraka-7003 -- Eureka集群
├── springcloud-study-provider-dept-8001 -- 构建服务提供者集群
├── springcloud-study-provider-dept-8002 -- 构建服务提供者集群
├── springcloud-study-provider-dept-8003 -- 构建服务提供者集群
├── springcloud-study-consumer-dept-80 -- 构建服务消费者
├── ribbon-service -- ribbon服务调用测试服务
├── hystrix-service -- hystrix服务调用测试服务
├── turbine-service -- 聚合收集hystrix实例监控信息的服务
├── hystrix-dashboard -- 展示hystrix实例监控信息的仪表盘
├── feign-service -- feign服务调用测试服务
├── zuul-proxy -- zuul作为网关的测试服务
├── config-server -- 配置中心服务
├── config-security-server -- 带安全认证的配置中心服务
└── config-client -- 获取配置的客户端服务
```

## 项目搭建

- 见工程中：[笔记.md](https://github.com/zpj80231/spring-cloud-study/blob/master/笔记.md) (非常详细)

## 项目启动

1. 启动euraka-service端集群：
   - [springcloud-study-euraka-7001](https://github.com/zpj80231/spring-cloud-study/tree/master/springcloud-study-euraka-7001)
   - [springcloud-study-euraka-7002](https://github.com/zpj80231/spring-cloud-study/tree/master/springcloud-study-euraka-7002)
   - [springcloud-study-euraka-7003](https://github.com/zpj80231/spring-cloud-study/tree/master/springcloud-study-euraka-7003)
   
2. 启动微服务提供者集群：
   - [springcloud-study-provider-dept-8001 (连01数据库)](https://github.com/zpj80231/spring-cloud-study/tree/master/springcloud-study-provider-dept-8001)
   - [springcloud-study-provider-dept-8002 (连02数据库)](https://github.com/zpj80231/spring-cloud-study/tree/master/springcloud-study-provider-dept-8002)
   - [springcloud-study-provider-dept-8003 (连03数据库)](https://github.com/zpj80231/spring-cloud-study/tree/master/springcloud-study-provider-dept-8003)
   
3. 启动为服务消费者：
   - [springcloud-study-consumer-dept-80 (含Ribbon客户端负载均衡)](https://github.com/zpj80231/spring-cloud-study/tree/master/springcloud-study-consumer-dept-80)
   