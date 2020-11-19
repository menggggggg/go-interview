# Golang 面试资料
## 序言

整理golang基础知识及linux、后端开发相关面试资料。

声明：未经许可，禁止原文转载。

## 目录

### golang

------

#### 数据类型

- string
- slice

[reslice](https://mp.weixin.qq.com/s/H3UzcKX2-Q4ywD_RJvMmEA)

- map

- interface

- channel

  [底层原理](https://mp.weixin.qq.com/s/tj02XI9L1dSKrUsy5E2OWg)

  [深度解密](https://mp.weixin.qq.com/s/lcenZGKTkAcTT7DZrhBbvw)

#### 内存分配

[分配器](https://mp.weixin.qq.com/s/TO_lmlFbVDgFmns9s_mMzw)

[变量分配到哪里](https://mp.weixin.qq.com/s/bZ06N2Cvl5HFxhDMMX1ReA)

#### 调度器

- goroutine

- G-P-M 模型 
  ![gmp](https://zhaomeng-private.oss-cn-shanghai.aliyuncs.com/images/gmp.png)

 [调度](https://mp.weixin.qq.com/s?__biz=MzA4ODg0NDkzOA==&mid=2247487174&amp;idx=1&amp;sn=a716cc5cc48b7cf6078698942a6c6c18&source=41&key=&ascene=14&uin=&devicetype=Windows+10&version=620603c8&lang=zh_CN&winzoom=1)

- 垃圾回收

#### 并发模型

- sync

  [sync.pool](https://mp.weixin.qq.com/s/6EuVw5rw7WdolZx_WWnr-Q)

#### 开源库

[go-zero](https://mp.weixin.qq.com/s/mrFnJpJzRa94W1mfGr7N1g)

[go-zero追踪](https://mp.weixin.qq.com/s/MlJRr3UZqRADyi15sHwPVA)

##### micro

```
(一)：入门 https://medium.com/@dche423/micro-in-action-getting-start-cn-99c870e078f 

(二)：项目结构与启动过程 https://medium.com/@dche423/micro-in-action-part2-cn-9bbc33d356eb 

(三)：调用服务 https://medium.com/@dche423/micro-in-action-call-service-cn-5ac679194636 

(四)：Pub/Sub https://medium.com/@dche423/micro-in-action-pub-sub-cn-ce010bffe1c 

(五)：Message Broker https://medium.com/@dche423/micro-in-action-5-message-broker-d975c2f28a55 

(六)：服务发现 https://medium.com/@dche423/micro-in-action-6-service-discovery-cn-c13c3e3829d 

(七)：熔断与限流 https://medium.com/@dche423/micro-in-action-7-cn-ce75d5847ef4 

(尾声): 分布式计划任务 https://medium.com/@dche423/micro-in-action-9-cron-job-dabec09058e1

```

#### 规范

[代码结构](https://mp.weixin.qq.com/s/yiU18PzHDxeCXc5YR5x9Ow)

[pprof](https://mp.weixin.qq.com/s/n8Ot6AWsat2gUCwlgoLRHg)

------

### linux

[内核图解](https://mp.weixin.qq.com/s/8XiqDofO0tI2dzxee4GyRw)

[读取文件发生了什么](https://mp.weixin.qq.com/s/A55BN5G7RBaLvCqKrizmdw)

[ CLOSE WAIT](https://mp.weixin.qq.com/s/sqBdycaClUixZQPgKy52Pw)

[epoll](https://mp.weixin.qq.com/s/zWaDVuNFfclx_sx_EuX63Q)

[负载均衡](https://mp.weixin.qq.com/s/0nW7Bpadgvq8NRRsTbZ3Vw)

#### nginx

[入门知识](https://mp.weixin.qq.com/s/fbvncZnPhFF7lqroFt0rqQ)

[日志配置](https://mp.weixin.qq.com/s/oSRVZ-2ucQBQ_IXYVXFk8g)

[高可用](https://mp.weixin.qq.com/s/li7AHGdDzjrAkuIoY0wcOQ)

------

### 网络知识

[字节实践](https://mp.weixin.qq.com/s/agIYfq_7Bu6WAJ-zJ2f1CQ)

[网络协议面试](https://mp.weixin.qq.com/s/_yEqNFbxsIhS_45WKTy9_w)

[TLS](https://mp.weixin.qq.com/s/pLBA220lkAj6Nb-Y-seLEw)

#### TCP

[必备知识点](https://mp.weixin.qq.com/s/THQ9zAJ4yso1knGtwKcw_Q)

#### HTTP

[缓存机制](https://mp.weixin.qq.com/s/1Eu0dGB2Eh35f0GXYz21aQ)

#### Grpc

[超时传递原理](https://mp.weixin.qq.com/s/9vA40m1wbQ8bBd_tO8B8IA)

------

### 数据库

[基础知识](https://mp.weixin.qq.com/s/I2qTMmAgLjt_1XX1UtiuzA)

[分库分表](https://mp.weixin.qq.com/s/CUkWPLdrdH2BJL0N7HFjvg)

[24个面试题](https://mp.weixin.qq.com/s/tb557BSaUvnN-mYX_lsTLw)

#### redis

[内存模型](https://mp.weixin.qq.com/s/YGmOoBZ7J-3dPrNntRTfSg)

[优化](https://mp.weixin.qq.com/s/NKGMTYCjsIga_1r2K3IPlw)

[开发规范](https://mp.weixin.qq.com/s/XO_mw76JoPUJP7WtKD1mbg)

[Redis缓存雪崩](https://mp.weixin.qq.com/s/g3DcfgF7vBd_n_ArOo8UTg)

[面试题1](https://mp.weixin.qq.com/s/Z4a8wbWvPDGFTkKJH0X9VQ)

#### mongo

[B/B+树](https://mp.weixin.qq.com/s/kRG8osOgLIenr7UeEqT7aQ)

[原子性](https://mp.weixin.qq.com/s/GoQg5FFG_5sDBVRF4OqDFA)

[优化指南](https://mp.weixin.qq.com/s/fA4Y69Xi7iZPdF8LwBSayg)

[优化指南2](https://mp.weixin.qq.com/s/izRaZ-oKXYAN1RFC8vWCMw)

------

### 微服务

[api 设计](https://mp.weixin.qq.com/s/IMXHaibmiskOBwZlk3wpiA)

------

### 消息队列

[Kafka](https://mp.weixin.qq.com/s/piD5ovHonJ6DiQm7fyXJvw)

[延时队列](https://mp.weixin.qq.com/s/qGywX7S8P3toy-RhQonDYQ)

[复习精讲](https://mp.weixin.qq.com/s/rzEX0wQCoDBxuFmws9f7Lw)

[消息投递](https://mp.weixin.qq.com/s/-jb-FAXzUVepTLFpmgZt8A)

[消息队列选型分析](https://mp.weixin.qq.com/s/6PcvA-8Kfb1LsFKN-ksZkA)

------

### ElasticSearch

[入门](https://mp.weixin.qq.com/s/gHTLSB1sBOlrJ3F8U9affQ)

[入门2](https://mp.weixin.qq.com/s/l20pmtgwuBUMv6JUdzXIbg)

[优化实战](https://mp.weixin.qq.com/s/PFzRT5Ky0reMXrMRJsj2jQ)

[优化实战2](https://mp.weixin.qq.com/s?__biz=MzA3ODIxNjYxNQ==&mid=2247487186&amp;idx=1&amp;sn=f64ab0c1597b6ae55b0b15229808f413&source=41&key=&ascene=14&uin=&devicetype=Windows+10&version=620603c8&lang=zh_CN&winzoom=1)

------

### 数据结构

[红黑树](https://mp.weixin.qq.com/s/gaOGm48mnONtV4wEE4uVCA)

[红黑树图解](https://mp.weixin.qq.com/s/kEaqW0FgzkU0X6UUQBm0-w)

[跳跃表](https://mp.weixin.qq.com/s/XY1gPvdV7hWTDYNDDW2zoQ)

------

### 高可用

[高性能](https://mp.weixin.qq.com/s/gsHiRnWdYNXnX4ycsRSAWA)

[熔断](https://mp.weixin.qq.com/s/n9wpL6uSjza2nEprLbJDKw)

[面试1](https://mp.weixin.qq.com/s/fHSKIgJVTdoPVu7hFAZXSw)

------

### 算法

[限流](https://mp.weixin.qq.com/s/Knx1dQ8L6cBx4HRUJ-EAUQ)

[限流2](https://mp.weixin.qq.com/s/68FSIEet5h3pI221iqIp4g)

[raft](https://mp.weixin.qq.com/s/ZYHZg-Ls6pD_Qr_wgKmcdA)

[图解raft](https://mp.weixin.qq.com/s/4Da9NEtDzNA70dU6e7CWGw)

[约瑟夫环](https://mp.weixin.qq.com/s/SpqjZSpaHiMhSb4vvljuJA)

------

### 设计模式

[mybatis中的9种](https://mp.weixin.qq.com/s/d_2Pom9BfgTHbQf2h8O0LA)

------

### 一致性

[一致性哈希](https://mp.weixin.qq.com/s/Q9MaeHXk6PPTOGfSFclURQ)

[面试1](https://mp.weixin.qq.com/s/VNr6pOygrzICXUi2YXRchA)

------

### 锁

[乐观锁与悲观锁](https://mp.weixin.qq.com/s/XO_mw76JoPUJP7WtKD1mbg)

------

### 模型

[权限设计](https://mp.weixin.qq.com/s/wox0f-bl9E7qAl3pXuuMTg)

[多租户](https://mp.weixin.qq.com/s/L6OKJK1ev1FyVDu03CQ0OA)

------

### kubernetes

[对象](https://mp.weixin.qq.com/s/qrJ50ma4LWBuOn_7WPGznw)

[干货文章100](https://mp.weixin.qq.com/s/8A_It3NNklbbG--P6Dw9gQ)

[pod创建](https://mp.weixin.qq.com/s/lcenZGKTkAcTT7DZrhBbvw)

[部署debug](https://donge.org/posts/envoy-vs-traefik/?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[[Envoy VS Traefik](https://donge.org/posts/envoy-vs-traefik/?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[最佳实践](https://mp.weixin.qq.com/s/CGcwPahTjjrDZZXHy_vKpA)

[50个面试问题](https://mp.weixin.qq.com/s/ctFbNctTbQEZixjKblfcyw)

[CI/CD](https://mp.weixin.qq.com/s/E21w94x7iu6BCY7dXF9-WQ)

[工具](https://mp.weixin.qq.com/s/DL2M_Y6ILIwtctm97ZisDA)

------

### 运维

[CI/CD](https://mp.weixin.qq.com/s/XDMXxM6A-S99Rf26OQH_hg)

[Devops](https://mp.weixin.qq.com/s/NWzUzX6wss7WeuVI_oFuHQ)

#### 监控

[监控体系](https://mp.weixin.qq.com/s/FGCZws3bQ9l9zOWDRTfdhg)

[监控工具](https://mp.weixin.qq.com/s/M-ygzU0V8hgITqx0Wdl6iQ)

------

### 面试题

[面试1](https://mp.weixin.qq.com/s/puhJymLO8IqMoHpzXR-d9w)

[面试2](https://mp.weixin.qq.com/s/pA2pYdoZU8ZIZoFm9txESw)

[面试3](https://mp.weixin.qq.com/s/dPDou-DKCYqzTHTHX6A0Bw)