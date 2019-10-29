# Spring Cloud学习笔记

## 觉得整理的不错的朋友，star一下哟，(*￣︶￣)

## 欢迎大家提问题交流

- 项目fork自gongxings/spring-cloud-study，基于自己的理解又添加了修改
- 这是gongxings的CSDN博客地址：https://blog.csdn.net/qq_18547653/article/details/88934787
博客能看到图片，效果比较好

![](images/springcloud架构图.png)

## 项目版本

- spring cloud版本：Dalston.SR1
- spring boot版本：1.5.19.RELEASE

## 项目模块说明

``` lua
spring-cloud-study
├── springcloud-study-api -- 构建公共子模块
├── springcloud-study-provider-dept-8001 -- 构建服务提供者
├── springcloud-study-consumer-dept-80 -- 构建服务消费者
├── springcloud-study-euraka-7001 -- Eureka集群
├── springcloud-study-euraka-7002 -- Eureka集群
├── springcloud-study-euraka-7003 -- Eureka集群
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

- 见工程中：笔记.md（非常详细）

## 项目启动

1. 启动euraka客户端集群：
   - springcloud-study-euraka-7001
   - springcloud-study-euraka-7001
   - springcloud-study-euraka-7001
   
2. 启动微服务提供者：
   - springcloud-study-provider-dept-8001
   
3. 启动为服务消费者：
   - springcloud-study-consumer-dept-80
   