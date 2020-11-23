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

[图解内存管理](https://mp.weixin.qq.com/s/CsHcVpZ_9rhO3aJy1-gBaA)

[内存管理分析](https://mp.weixin.qq.com/s/rydO2JK-r8JjG9v_Uy7gXg)

[变量分配到哪里](https://mp.weixin.qq.com/s/bZ06N2Cvl5HFxhDMMX1ReA)

#### 调度器

- goroutine

  [goroutine 泄露](https://mp.weixin.qq.com/s/5q5eIMDHz35ycTBTkB33JQ)

- G-P-M 模型 
  ![gmp](https://zhaomeng-private.oss-cn-shanghai.aliyuncs.com/images/gmp.png)

 [调度](https://mp.weixin.qq.com/s?__biz=MzA4ODg0NDkzOA==&mid=2247487174&amp;idx=1&amp;sn=a716cc5cc48b7cf6078698942a6c6c18&source=41&key=&ascene=14&uin=&devicetype=Windows+10&version=620603c8&lang=zh_CN&winzoom=1)

- 垃圾回收

[三色标记法](https://mp.weixin.qq.com/s/TqNLZoQQhJeech7RWnvtfA)

#### 并发模型

- sync

  [sync.pool](https://mp.weixin.qq.com/s/6EuVw5rw7WdolZx_WWnr-Q)

#### 单元测试

[详解](https://mp.weixin.qq.com/s/eAptnygPQcQ5Ex8-6l0byA)

[压测](https://www.instana.com/blog/practical-golang-benchmarks/)

[误区与实践](https://mp.weixin.qq.com/s/k8WNWpCIVl4xTmP3TQ_gxQ)

#### 开源库

[go-zero](https://mp.weixin.qq.com/s/mrFnJpJzRa94W1mfGr7N1g)

[go-zero追踪](https://mp.weixin.qq.com/s/MlJRr3UZqRADyi15sHwPVA)

[jupiter](http://jupiter.douyu.com/jupiter/)

[别人代码学习golang](https://syncd.cn/study_code_01/)

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

[uber代码规范](https://github.com/xxjwxc/uber_go_guide_cn)

[go-advice](https://github.com/cristaloleg/go-advice/blob/master/README_ZH.md)

[代码结构](https://mp.weixin.qq.com/s/yiU18PzHDxeCXc5YR5x9Ow)

[热重启](https://mp.weixin.qq.com/s/UVZKFmv8p4ghm8ICdz85wQ)

[性能优化](https://mp.weixin.qq.com/s?__biz=MzAxMTA4Njc0OQ==&mid=2651439572&idx=1&sn=8e550f66eae78e2838e441b07a0330dc&chksm=80bb1f26b7cc9630f1144c135a4a448f8688d42e47ec1b64d90f9a76d427f69ae70c455b008f&scene=21#wechat_redirect)

[高阶调试技巧](https://mp.weixin.qq.com/s/GJxHVbaVXnHussFXf1tDMQ)

[pprof](https://mp.weixin.qq.com/s/n8Ot6AWsat2gUCwlgoLRHg)

------

### linux

[操作系统](https://mp.weixin.qq.com/s/mC_zZuMBYd5FdmI241uqqQ)

[内核图解](https://mp.weixin.qq.com/s/8XiqDofO0tI2dzxee4GyRw)

[基础概念](https://mp.weixin.qq.com/s/BNUMqP4xBTKTmZRhbS-iwg)

[如何写出让CPU跑的更快的代码](https://mp.weixin.qq.com/s/-uhAhBD2zGl_h19E4fNJzQ)

[读取文件发生了什么](https://mp.weixin.qq.com/s/A55BN5G7RBaLvCqKrizmdw)

[ CLOSE WAIT](https://mp.weixin.qq.com/s/sqBdycaClUixZQPgKy52Pw)

[epoll](https://mp.weixin.qq.com/s/zWaDVuNFfclx_sx_EuX63Q)

[负载均衡](https://mp.weixin.qq.com/s/0nW7Bpadgvq8NRRsTbZ3Vw)

[eBPF](https://mp.weixin.qq.com/s/25mhUrNhF3HW8H6-ES7waA)

#### nginx

[入门知识](https://mp.weixin.qq.com/s/fbvncZnPhFF7lqroFt0rqQ)

[日志配置](https://mp.weixin.qq.com/s/oSRVZ-2ucQBQ_IXYVXFk8g)

[高可用](https://mp.weixin.qq.com/s/li7AHGdDzjrAkuIoY0wcOQ)

------

### 网络知识

[基础知识](https://mp.weixin.qq.com/s/JBsqCQAouQ6hH7gcvtYMLg)

[字节实践](https://mp.weixin.qq.com/s/agIYfq_7Bu6WAJ-zJ2f1CQ)

[网络协议面试](https://mp.weixin.qq.com/s/_yEqNFbxsIhS_45WKTy9_w)

[TLS](https://mp.weixin.qq.com/s/pLBA220lkAj6Nb-Y-seLEw)

[TLS/SSL](https://mp.weixin.qq.com/s?__biz=MzUyMDk2MzUzMQ==&mid=2247485794&idx=1&sn=28c414b56e899389c4101919ccfdf9c3&chksm=f9e31dc6ce9494d080b5135095aa30b3f30cb3337c4105ba8ef47dfc5ef74c8acd6f95926657&token=681607169&lang=zh_CN#rd)

[文件上传](https://mp.weixin.qq.com/s/sHqN9sf8iOLzKApH0KR9vg)

[文件断点续传](https://mp.weixin.qq.com/s/bI5xYq3jUtp-sviKlzHtNg)

#### TCP

[必备知识点](https://mp.weixin.qq.com/s/THQ9zAJ4yso1knGtwKcw_Q)

[三次握手](https://mp.weixin.qq.com/s/GQTVytNus8EcoGEkOSTUog)

[23个问题](https://mp.weixin.qq.com/s?__biz=MzkxNTE3NjQ3MA==&mid=2247485731&idx=1&sn=5b95cefa09ef1e72a8010339654b0e5d&source=41#wechat_redirect)

[问题排查1](https://mp.weixin.qq.com/s/iBk-kEj2tJqMCuFOdXCLEA)

[粘包处理](https://zhuanlan.zhihu.com/p/156893094?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[keep-alive keepalive](https://zhuanlan.zhihu.com/p/224595048?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[IO多路复用](https://mp.weixin.qq.com/s/PzOF9lFYVacPIRx0JakTjA)

[最大并发数](https://mp.weixin.qq.com/s/zb8DdjVn-f1zc51evyZ_eg)

#### HTTP

[http.client 源码剖析](https://mp.weixin.qq.com/s/JMdDu105ux9GFV1S11jE7w)

[缓存机制](https://mp.weixin.qq.com/s/1Eu0dGB2Eh35f0GXYz21aQ)

[谈谈Http](https://zhuanlan.zhihu.com/p/159274359?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

#### Grpc

[超时传递原理](https://mp.weixin.qq.com/s/9vA40m1wbQ8bBd_tO8B8IA)

#### Websocket

[websocket](https://mp.weixin.qq.com/s/28FSBp4lj2l1H0caMNrjrw)

------

### 数据库

[基础知识](https://mp.weixin.qq.com/s/I2qTMmAgLjt_1XX1UtiuzA)

[索引](https://mp.weixin.qq.com/s/5Yl6H6up9ntZq6l8qxiogw)

[分库分表](https://mp.weixin.qq.com/s/CUkWPLdrdH2BJL0N7HFjvg)

[24个面试题](https://mp.weixin.qq.com/s/tb557BSaUvnN-mYX_lsTLw)

[拓展字段设计](http://blog.bytearch.com/2020/04/23/field-extension/?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

#### redis

[内存模型](https://mp.weixin.qq.com/s/YGmOoBZ7J-3dPrNntRTfSg)

[优化](https://mp.weixin.qq.com/s/NKGMTYCjsIga_1r2K3IPlw)

[开发规范](https://mp.weixin.qq.com/s/XO_mw76JoPUJP7WtKD1mbg)

[主从服务机制](https://www.jianshu.com/p/58a48397b931?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[redis cluster原理](https://mp.weixin.qq.com/s/bDg3Y1hBnK0ac9_uquu9Yw)

[Redis缓存雪崩](https://mp.weixin.qq.com/s/g3DcfgF7vBd_n_ArOo8UTg)

[客户端缓存](https://mp.weixin.qq.com/s/Mc9SpVeuRIe8Pi2HkPQWjQ)

[缓存更新](https://mp.weixin.qq.com/s/9GeYSVvKMtKGpTyBWTs_Zw)

[数据同步](https://mp.weixin.qq.com/s/RBEuvvaLVgmarXqG7Hc4Qw)

[为什么这么快](https://mp.weixin.qq.com/s/b_yzbLeQh57oYjqlIgPiYQ)

[集群搭建总结](https://mp.weixin.qq.com/s?__biz=MzUzNjAxODg4MQ==&mid=2247485567&idx=1&sn=0644277d2c046890a14442830a4ed0f3&chksm=fafde2d1cd8a6bc70307efef696654f89074c2219f824af72effe5eb027cee983b364e4279c8&token=2145573189&lang=zh_CN#rd)

[面试题1](https://mp.weixin.qq.com/s/Z4a8wbWvPDGFTkKJH0X9VQ)

#### mongo

[B/B+树](https://mp.weixin.qq.com/s/kRG8osOgLIenr7UeEqT7aQ)

[原子性](https://mp.weixin.qq.com/s/GoQg5FFG_5sDBVRF4OqDFA)

[技术从0到1](https://mp.weixin.qq.com/s/FrEqtjMQeQnRvDX6zO1Bhw)

[文件存储](https://mp.weixin.qq.com/s/wXnExtpQAuV9OV3KbWVCwQ)

[优化指南](https://mp.weixin.qq.com/s/fA4Y69Xi7iZPdF8LwBSayg)

[优化指南2](https://mp.weixin.qq.com/s/izRaZ-oKXYAN1RFC8vWCMw)

------

### 微服务

[api 设计](https://mp.weixin.qq.com/s/IMXHaibmiskOBwZlk3wpiA)

------

### 消息队列

[Kafka](https://mp.weixin.qq.com/s/piD5ovHonJ6DiQm7fyXJvw)

[面试角度学Kafka](https://mp.weixin.qq.com/s/QF9b9vpncLS24xMzFkanTQ)

[rabbitmq](https://mp.weixin.qq.com/s/qSBaD1MInJrvl23kOeeMeA)

[延时队列](https://mp.weixin.qq.com/s/qGywX7S8P3toy-RhQonDYQ)

[复习精讲](https://mp.weixin.qq.com/s/rzEX0wQCoDBxuFmws9f7Lw)

[消息投递](https://mp.weixin.qq.com/s/-jb-FAXzUVepTLFpmgZt8A)

[消息队列选型分析](https://mp.weixin.qq.com/s/6PcvA-8Kfb1LsFKN-ksZkA)

[设计难题](https://mp.weixin.qq.com/s/C1tgYwiBoRJY3A7_WAP20w)

[写个消息中间件](https://mp.weixin.qq.com/s?__biz=MzkxNTE3NjQ3MA==&mid=2247485721&idx=1&sn=a30a9be1685d88c61d7dc5722d50d9c3&source=41#wechat_redirect)

[面试连环问](https://mp.weixin.qq.com/s?__biz=MzkxNTE3NjQ3MA==&mid=2247485753&idx=1&sn=d22f8adc8eb0dfc08163e160127f6b17&source=41#wechat_redirect)

------

### ElasticSearch

[入门](https://mp.weixin.qq.com/s/gHTLSB1sBOlrJ3F8U9affQ)

[入门2](https://mp.weixin.qq.com/s/l20pmtgwuBUMv6JUdzXIbg)

[常见错误及最佳实践](https://mp.weixin.qq.com/s/zsAk7clgxzrjWLpQbYoTXg)

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

[链表题](https://mp.weixin.qq.com/s/Ym7MhhJ--NcaRRnj1y1vFA)

[限流](https://mp.weixin.qq.com/s/Knx1dQ8L6cBx4HRUJ-EAUQ)

[限流2](https://mp.weixin.qq.com/s/68FSIEet5h3pI221iqIp4g)

[raft](https://mp.weixin.qq.com/s/ZYHZg-Ls6pD_Qr_wgKmcdA)

[图解raft](https://mp.weixin.qq.com/s/4Da9NEtDzNA70dU6e7CWGw)

[约瑟夫环](https://mp.weixin.qq.com/s/SpqjZSpaHiMhSb4vvljuJA)

[雪花算法](https://mp.weixin.qq.com/s/5OQ-ZXUnbbT864ZVF8pC_g)

------

### 加密

[常见加密算法](https://mp.weixin.qq.com/s/x_y6w-F1lCN102E8KQmuvQ)

------

### 设计模式

[go设计模式代码实现](http://lailin.xyz/post/singleton.html)

[go设计模式](https://mp.weixin.qq.com/s/VZfwNlqSLzCK0hWSfG4Yzw)

[图解9种常见设计模式](https://mp.weixin.qq.com/s/-jpIitC1j3geciJzkuexdA)

[mybatis中的9种](https://mp.weixin.qq.com/s/d_2Pom9BfgTHbQf2h8O0LA)

------

### 一致性

[一致性哈希](https://mp.weixin.qq.com/s/Q9MaeHXk6PPTOGfSFclURQ)

[面试1](https://mp.weixin.qq.com/s/VNr6pOygrzICXUi2YXRchA)

------

### 锁

[乐观锁与悲观锁](https://mp.weixin.qq.com/s/XO_mw76JoPUJP7WtKD1mbg)

[锁的应用场景](https://mp.weixin.qq.com/s/HH4ov97JkukLFg4EyPuzsQ)

------

### 模型

[常见登录鉴权](https://zhuanlan.zhihu.com/p/271768645?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[权限设计](https://mp.weixin.qq.com/s/wox0f-bl9E7qAl3pXuuMTg)

[分布式session](https://mp.weixin.qq.com/s/MdtC9CExp-WkNN27x66r0w)

[多租户](https://mp.weixin.qq.com/s/L6OKJK1ev1FyVDu03CQ0OA)

[腾讯网关](https://mp.weixin.qq.com/s/NxVIAxQw2ywKURdK4lpx9w)

[依赖注入](https://blog.wangke.io/articles/01fe3063_%E4%B8%80%E6%96%87%E8%AF%B4%E9%80%8F_%E4%BE%9D%E8%B5%96%E6%B3%A8%E5%85%A5_?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[连接池](https://mp.weixin.qq.com/s/90fQiMReB4OvWMDwA_xq_Q)

[链路追踪](https://mp.weixin.qq.com/s/P12ivKCMRckx55s5vtf37A)

[GraphQL](https://mp.weixin.qq.com/s?__biz=MzA4Nzc4MjI4MQ==&mid=2652404013&idx=1&sn=a259af0c9cd667ea860801aabb97dbc3&chksm=8bd8ffcbbcaf76dd763a1796928cc0e73f7af5517415c050959358a6c4a4390612abdfea642b&token=2128286661&lang=zh_CN#rd)

[数据中台](https://mp.weixin.qq.com/s/NIG5PfWMwWRpPgQVti3xqA)

[推荐系统](https://mp.weixin.qq.com/s/yQavfvBayYbMEc7c9ObMxg)

[稳定性规范](https://mp.weixin.qq.com/s/gVNKibDQ6UsX_q8_CHvg1A)

[优雅向前兼容](https://mp.weixin.qq.com/s/2PMte2zhaf9tUmMvHiEwxw)

------

### kubernetes

[入门](http://matt33.com/2020/08/02/kubernetes-start/?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[对象](https://mp.weixin.qq.com/s/qrJ50ma4LWBuOn_7WPGznw)

[干货文章100](https://mp.weixin.qq.com/s/8A_It3NNklbbG--P6Dw9gQ)

[pod 入门指南](https://mp.weixin.qq.com/s/igpOZUszs8sNT4_226bnwA)

[pod创建](https://mp.weixin.qq.com/s/lcenZGKTkAcTT7DZrhBbvw)

[部署debug](https://donge.org/posts/envoy-vs-traefik/?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[[Envoy VS Traefik](https://donge.org/posts/envoy-vs-traefik/?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[Envoy 几种负责均衡算法](https://mp.weixin.qq.com/s/Yxo4tua34w2O5BDNVtFm2w)

[最佳实践](https://mp.weixin.qq.com/s/CGcwPahTjjrDZZXHy_vKpA)

[50个面试问题](https://mp.weixin.qq.com/s/ctFbNctTbQEZixjKblfcyw)

[CI/CD](https://mp.weixin.qq.com/s/E21w94x7iu6BCY7dXF9-WQ)

[工具](https://mp.weixin.qq.com/s/DL2M_Y6ILIwtctm97ZisDA)

#### Istio

[简介](http://jartto.wang/2020/07/29/istio-1/?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

------

### 运维

[CI/CD](https://mp.weixin.qq.com/s/XDMXxM6A-S99Rf26OQH_hg)

[Devops](https://mp.weixin.qq.com/s/NWzUzX6wss7WeuVI_oFuHQ)

#### 监控

[监控告警](https://mp.weixin.qq.com/s/qaNWBlDGgE2hNnu6SV4EBg)

[监控体系](https://mp.weixin.qq.com/s/FGCZws3bQ9l9zOWDRTfdhg)

[监控工具](https://mp.weixin.qq.com/s/M-ygzU0V8hgITqx0Wdl6iQ)

[prometheus微服务监控](https://mp.weixin.qq.com/s/mbR_VX2G-exNRGKmwqqshA)

------

### 面试题

[简历与项目介绍](https://mp.weixin.qq.com/s/phLXpzW6Vz7llcWijjmMUg)

[面试1](https://mp.weixin.qq.com/s/puhJymLO8IqMoHpzXR-d9w)

[面试2](https://mp.weixin.qq.com/s/pA2pYdoZU8ZIZoFm9txESw)

[面试3](https://mp.weixin.qq.com/s/dPDou-DKCYqzTHTHX6A0Bw)