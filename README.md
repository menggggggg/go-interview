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

[struct](https://mp.weixin.qq.com/s/QnMOwYUANdydbiM8yGznHA)

[看Go中的struct如何被优化](https://mp.weixin.qq.com/s/maJjOhoByeEA1j_btdpBgg)

[反射](https://mp.weixin.qq.com/s/TmzV2VTfkE8of2_zuKa0gAs)

#### 内存分配

[分配器](https://mp.weixin.qq.com/s/TO_lmlFbVDgFmns9s_mMzw)

[内存分配扒得干干净净](https://mp.weixin.qq.com/s/8_aeGLEsTItXF3RSpj4T2g)

[图解内存管理](https://mp.weixin.qq.com/s/CsHcVpZ_9rhO3aJy1-gBaA)

[内存管理分析](https://mp.weixin.qq.com/s/rydO2JK-r8JjG9v_Uy7gXg)

[变量分配到哪里](https://mp.weixin.qq.com/s/bZ06N2Cvl5HFxhDMMX1ReA)

[内存逃逸](https://mp.weixin.qq.com/s/MepbrrSlGVhNrEkTQhfhhQ)

[内存分配（性能优化）](https://mp.weixin.qq.com/s/Dtl7INEA2tnm1ZjSODwazg)

[本地内存](https://mp.weixin.qq.com/s/lAE7im2NSZm-I_7BdVlFng)

#### 调度器

- goroutine

  [goroutine 泄露](https://mp.weixin.qq.com/s/5q5eIMDHz35ycTBTkB33JQ)

  [性能分析](https://mp.weixin.qq.com/s/zEtK5uAd40vD-hcWrQDsmw)

- G-P-M 模型 
  ![gmp](https://zhaomeng-private.oss-cn-shanghai.aliyuncs.com/images/gmp.png)

 [调度](https://mp.weixin.qq.com/s?__biz=MzA4ODg0NDkzOA==&mid=2247487174&amp;idx=1&amp;sn=a716cc5cc48b7cf6078698942a6c6c18&source=41&key=&ascene=14&uin=&devicetype=Windows+10&version=620603c8&lang=zh_CN&winzoom=1)

- 垃圾回收

[Go垃圾回收、三色标记原理](https://mp.weixin.qq.com/s/srY28v3U-hDr_brV4_BWww)

[白话Go的垃圾回收原理](https://mp.weixin.qq.com/s/s8_RWA_D-I03AnBZNF9utg)

[漫画](https://mp.weixin.qq.com/s/FQ25hro703sSNYTp-vfAwg)

[GC 20问](https://mp.weixin.qq.com/s/5xjH-LJ53XiNm2sMNQZiGQ)

#### 并发模型

[流水线模型](https://mp.weixin.qq.com/s/IuGaKbQvW7z1KsoMhB8mgg)

[golang 5种原子操作](https://juejin.cn/post/7010590496204521485?utm_source=gold_browser_extension)

- sync

  [sync.pool](https://mp.weixin.qq.com/s/6EuVw5rw7WdolZx_WWnr-Q)

#### 单元测试

[详解](https://mp.weixin.qq.com/s/eAptnygPQcQ5Ex8-6l0byA)

[手把手教你如何进行 Golang 单元测试](https://mp.weixin.qq.com/s/N5wby-aWWEPc7mHN_lN3lQ)

[压测](https://www.instana.com/blog/practical-golang-benchmarks/)

[误区与实践](https://mp.weixin.qq.com/s/k8WNWpCIVl4xTmP3TQ_gxQ)

[最佳实践](https://mp.weixin.qq.com/s/DbKXka598YVDJHSFCcQOSQ)

[Go Test小技巧](https://mp.weixin.qq.com/s/y3UKaLD40A7C89GkGq7GKQ)

#### 调试

[golang 调试分析的高阶技巧](https://mp.weixin.qq.com/s/j0ZWlctxzx_yNhJb__hciA)

[如何保留 Go 程序崩溃现场](https://mp.weixin.qq.com/s/RktnMydDtOZFwEFLLYzlCA)

#### 开源库

[go-zero](https://mp.weixin.qq.com/s/mrFnJpJzRa94W1mfGr7N1g)

[go-zero追踪](https://mp.weixin.qq.com/s/MlJRr3UZqRADyi15sHwPVA)

[jupiter](http://jupiter.douyu.com/jupiter/)

[别人代码学习golang](https://syncd.cn/study_code_01/)

[分布式事务（dtm）](https://mp.weixin.qq.com/s/UmGnCM3SLWZUI0yMaTeqxA)

[会话控制](https://github.com/gorilla/sessions)

[解读Zap的高性能](https://mp.weixin.qq.com/s/Qc5tGELKPZOA9LEBOEkuow)

[http 重试](https://mp.weixin.qq.com/s/DAEZQnC2UYwcFeEh0e8VoQ)

[Go 语言官方依赖注入工具 Wire](https://mp.weixin.qq.com/s/yHB9BzEGIki1fyjYojdpYQ)

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

##### gin

https://mp.weixin.qq.com/s/935NOIg4GzRsupZefwqWeA

#### 规范

[uber代码规范](https://github.com/xxjwxc/uber_go_guide_cn)

[go-advice](https://github.com/cristaloleg/go-advice/blob/master/README_ZH.md)

[代码结构](https://mp.weixin.qq.com/s/yiU18PzHDxeCXc5YR5x9Ow)

[浅谈如何组织Go代码结构](https://mp.weixin.qq.com/s/9_WQUpvHKli4btPqCA89Aw)

[编程模式](https://mp.weixin.qq.com/s/0yLVkQ4kJLlvk5Vfz0lQkA)

[热重启](https://mp.weixin.qq.com/s/UVZKFmv8p4ghm8ICdz85wQ)

[性能优化](https://mp.weixin.qq.com/s?__biz=MzAxMTA4Njc0OQ==&mid=2651439572&idx=1&sn=8e550f66eae78e2838e441b07a0330dc&chksm=80bb1f26b7cc9630f1144c135a4a448f8688d42e47ec1b64d90f9a76d427f69ae70c455b008f&scene=21#wechat_redirect)

[高阶调试技巧](https://mp.weixin.qq.com/s/GJxHVbaVXnHussFXf1tDMQ)

[pprof](https://mp.weixin.qq.com/s/n8Ot6AWsat2gUCwlgoLRHg)

[Profiling 在微服务应用下的落地实践](https://mp.weixin.qq.com/s/vYTU2FjJXWD7cxwlKTco0g)

[Go 应用优化指北](https://mp.weixin.qq.com/s/KFT1hw02Zih1TMMlDWztCQ)

[Go 适合 IO 密集型？并不准确](https://mp.weixin.qq.com/s/xDXwsVjOfU2j3gisiHTZTQ)

[Context这三个应用场景](https://mp.weixin.qq.com/s/uIL7gsdUn89MopbAxE2rjQ)

[Context包详解](https://mp.weixin.qq.com/s/_5gBIwvtXKJME7AV2W2bqQ)

[Go 组件 Context 源码学习笔记](https://mp.weixin.qq.com/s/PoXSEDHRyKCyjibFGS0wHw)

[一套优雅的 Go 错误问题解决方案](https://mp.weixin.qq.com/s/RFF2gSikqXiWXIaOxQZsxQ)

[错误处理的一些建议](https://mp.weixin.qq.com/s/T4CCs7r1COUq-mCnlfCJCQ)

[Go 只会 if err != nil？这是不对的，分享这些优雅的处理姿势给你！](https://mp.weixin.qq.com/s/_oO-EZXZq8kUWxvJpdOGDA)

[不想Go 错误处理太臃肿](https://mp.weixin.qq.com/s/9UiLG_co8k8SXbRUxE1SNw)

[22条API设计的最佳实践](https://mp.weixin.qq.com/s/doQsjLpZ4F68GtK7XR5QDQ)

[google最佳实践](https://mp.weixin.qq.com/s/XftPV6aiaiqKFCVtM4hhQA)

------

### linux

[操作系统](https://mp.weixin.qq.com/s/mC_zZuMBYd5FdmI241uqqQ)

[内核图解](https://mp.weixin.qq.com/s/8XiqDofO0tI2dzxee4GyRw)

[基础概念](https://mp.weixin.qq.com/s/BNUMqP4xBTKTmZRhbS-iwg)

[如何写出让CPU跑的更快的代码](https://mp.weixin.qq.com/s/-uhAhBD2zGl_h19E4fNJzQ)

[读取文件发生了什么](https://mp.weixin.qq.com/s/A55BN5G7RBaLvCqKrizmdw)

[ CLOSE WAIT](https://mp.weixin.qq.com/s/sqBdycaClUixZQPgKy52Pw)

[epoll](https://mp.weixin.qq.com/s/zWaDVuNFfclx_sx_EuX63Q)

[Linux epoll惊群问题](https://mp.weixin.qq.com/s/O_QVxhyS7C3gJluqaLerWQ)

[负载均衡](https://mp.weixin.qq.com/s/0nW7Bpadgvq8NRRsTbZ3Vw)

[eBPF](https://mp.weixin.qq.com/s/25mhUrNhF3HW8H6-ES7waA)

[深入理解netfilter框架](https://github.com/0voice/campus_recruitmen_questions)

[深入理解Linux IO模型](https://mp.weixin.qq.com/s/PIIwZH5fQiaXQQmhYGCo7g)

[同步？异步？阻塞？非阻塞？多路复用？](https://mp.weixin.qq.com/s/OT9goRL6JSGl70DtF7a31Q)

[IO多路复用 select/poll/epoll 实现原理](https://mp.weixin.qq.com/s/5xj42JPKG8o5T7hjXIKywg)

[深入了解零拷贝](https://mp.weixin.qq.com/s/j1KjR5bRQV6oGrU5tsyHgg)

[当谈论协程时，我们在谈论什么](https://mp.weixin.qq.com/s/IO4ynnKEfy2Rt-Me7EIeqg)

[​浅谈协程](https://mp.weixin.qq.com/s/SyWjLg3lYx3pIJQfEtik8Q)

#### nginx

[入门知识](https://mp.weixin.qq.com/s/fbvncZnPhFF7lqroFt0rqQ)

[日志配置](https://mp.weixin.qq.com/s/oSRVZ-2ucQBQ_IXYVXFk8g)

[高可用](https://mp.weixin.qq.com/s/li7AHGdDzjrAkuIoY0wcOQ)

------

### 网络知识

[基础知识](https://mp.weixin.qq.com/s/JBsqCQAouQ6hH7gcvtYMLg)

[基础知识2](https://mp.weixin.qq.com/s/cHVsxIDPo8wXPTqvvdnvXQ)

[UDP就一定比TCP快吗？](https://mp.weixin.qq.com/s/TCsl-gee8U0hCp0f914xZQ)

[详解网络基础知识](https://mp.weixin.qq.com/s/MKfVBi9GwgY6qxVwxmsCcg)

[Linux网络IO精华指南](https://mp.weixin.qq.com/mp/profile_ext?action=home&__biz=MjM5ODYwMjI2MA==&scene=161#wechat_redirect)

[字节实践](https://mp.weixin.qq.com/s/agIYfq_7Bu6WAJ-zJ2f1CQ)

[网络协议面试](https://mp.weixin.qq.com/s/_yEqNFbxsIhS_45WKTy9_w)

[TLS](https://mp.weixin.qq.com/s/pLBA220lkAj6Nb-Y-seLEw)

[TLS/SSL](https://mp.weixin.qq.com/s?__biz=MzUyMDk2MzUzMQ==&mid=2247485794&idx=1&sn=28c414b56e899389c4101919ccfdf9c3&chksm=f9e31dc6ce9494d080b5135095aa30b3f30cb3337c4105ba8ef47dfc5ef74c8acd6f95926657&token=681607169&lang=zh_CN#rd)

[文件上传](https://mp.weixin.qq.com/s/sHqN9sf8iOLzKApH0KR9vg)

[文件断点续传](https://mp.weixin.qq.com/s/bI5xYq3jUtp-sviKlzHtNg)

[常见网络编程面试题](https://mp.weixin.qq.com/s/NhUUl4VxzsoNkvv7roBRPg)

[面试题集锦](https://mp.weixin.qq.com/s/AaZlb_cKsHb47q7WUiP3IQ)

[SSH](https://mp.weixin.qq.com/s/GdbR83cv7HQeSd8aH5_QDQ)

[能ping通，TCP就一定能连通吗？](https://mp.weixin.qq.com/s/fb2uUWz5ZjPEfYv_l6e4Zg)

#### TCP

[了解 HTTP 看这一篇就够](https://mp.weixin.qq.com/s/JVQPy8hAVoq1pRq63HKBOw)

[必备知识点](https://mp.weixin.qq.com/s/THQ9zAJ4yso1knGtwKcw_Q)

[三次握手](https://mp.weixin.qq.com/s/GQTVytNus8EcoGEkOSTUog)

[三次握手2](https://mp.weixin.qq.com/s/U0_kldMWChgCZxoYKyVRZQ)

[深入理解 Linux 的 TCP 三次握手](https://mp.weixin.qq.com/s/G2LuRZjQE15F6fSU-Bv_jw)

[23个问题](https://mp.weixin.qq.com/s?__biz=MzkxNTE3NjQ3MA==&mid=2247485731&idx=1&sn=5b95cefa09ef1e72a8010339654b0e5d&source=41#wechat_redirect)

[问题排查1](https://mp.weixin.qq.com/s/iBk-kEj2tJqMCuFOdXCLEA)

[粘包处理](https://zhuanlan.zhihu.com/p/156893094?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[keep-alive keepalive](https://zhuanlan.zhihu.com/p/224595048?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[IO多路复用](https://mp.weixin.qq.com/s/PzOF9lFYVacPIRx0JakTjA)

[IO多路复用2](https://mp.weixin.qq.com/s?__biz=MzI0MjEwMDMzNQ==&mid=2652517896&idx=1&sn=0ccd0ddf7e0b75094a6843039948692f&chksm=f2efe708c5986e1e00e33dc17e063e9398d1a54a7c2b5eee94de7a99be912e8edb42cb133b86&token=847914524&lang=zh_CN#rd)

[最大并发数](https://mp.weixin.qq.com/s/zb8DdjVn-f1zc51evyZ_eg)

#### HTTP

[http.client 源码剖析](https://mp.weixin.qq.com/s/JMdDu105ux9GFV1S11jE7w)

[缓存机制](https://mp.weixin.qq.com/s/1Eu0dGB2Eh35f0GXYz21aQ)

[谈谈Http](https://zhuanlan.zhihu.com/p/159274359?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[一个故事看懂HTTPS](https://juejin.cn/post/6995162794161094663)

#### Grpc

[超时传递原理](https://mp.weixin.qq.com/s/9vA40m1wbQ8bBd_tO8B8IA)

[gRPC 基础概念详解](https://mp.weixin.qq.com/s/I2QHEBO26nGqhGwIw281Pg)

[既然有HTTP协议，为什么还要有RPC](https://mp.weixin.qq.com/s/0QWxFylodn7T6nvcS6HsDg)

#### Websocket

[websocket](https://mp.weixin.qq.com/s/28FSBp4lj2l1H0caMNrjrw)

[分布式解决方案](https://mp.weixin.qq.com/s/QeWb-9-j5EYeB7I37gZ50A)

------

### 数据库

[基础知识](https://mp.weixin.qq.com/s/I2qTMmAgLjt_1XX1UtiuzA)

[索引](https://mp.weixin.qq.com/s/5Yl6H6up9ntZq6l8qxiogw)

[分库分表](https://mp.weixin.qq.com/s/CUkWPLdrdH2BJL0N7HFjvg)

[分库分表后如何设计索引](https://mp.weixin.qq.com/s/H6DUHf985dZ7hoiitsK2bg)

[24个面试题](https://mp.weixin.qq.com/s/tb557BSaUvnN-mYX_lsTLw)

[拓展字段设计](http://blog.bytearch.com/2020/04/23/field-extension/?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[慢 SQL 分析与优化](https://mp.weixin.qq.com/s/CaSVhAJgycjjbCxAkII2ZA)

[海量数据冷热分离方案与实践](https://mp.weixin.qq.com/s/ZKRkZP6rLHuTE1wvnqmAPQ)

[为什么说mysql数据库单表最大两千万](https://mp.weixin.qq.com/s/mWsDaMb8LTFf8M5eiT89Sg)
#### redis

[内存模型](https://mp.weixin.qq.com/s/YGmOoBZ7J-3dPrNntRTfSg)

[Redis 竟然浪费了这么多内存](https://mp.weixin.qq.com/s/S8e7fXL0rO3pOS_QRp44iA)

[带你走进 Redis](https://mp.weixin.qq.com/s/4bAPVdUr_XbIw9xFCtWhfw)

[优化](https://mp.weixin.qq.com/s/NKGMTYCjsIga_1r2K3IPlw)

[开发规范](https://mp.weixin.qq.com/s/XO_mw76JoPUJP7WtKD1mbg)

[主从服务机制](https://www.jianshu.com/p/58a48397b931?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[redis cluster原理](https://mp.weixin.qq.com/s/bDg3Y1hBnK0ac9_uquu9Yw)

[Redis缓存雪崩](https://mp.weixin.qq.com/s/g3DcfgF7vBd_n_ArOo8UTg)

[客户端缓存](https://mp.weixin.qq.com/s/Mc9SpVeuRIe8Pi2HkPQWjQ)

[缓存更新](https://mp.weixin.qq.com/s/9GeYSVvKMtKGpTyBWTs_Zw)

[数据同步](https://mp.weixin.qq.com/s/RBEuvvaLVgmarXqG7Hc4Qw)

[讲透数据库缓存一致性问题](https://mp.weixin.qq.com/s/U87wrGsx0Eop3CbF9mlTwQ)

[为什么这么快](https://mp.weixin.qq.com/s/b_yzbLeQh57oYjqlIgPiYQ)

[为什么这么快2](https://juejin.cn/post/6915599025882431501?utm_source=gold_browser_extension#heading-4)

[集群搭建总结](https://mp.weixin.qq.com/s?__biz=MzUzNjAxODg4MQ==&mid=2247485567&idx=1&sn=0644277d2c046890a14442830a4ed0f3&chksm=fafde2d1cd8a6bc70307efef696654f89074c2219f824af72effe5eb027cee983b364e4279c8&token=2145573189&lang=zh_CN#rd)

[缓存设计的好，服务基本不会倒](https://mp.weixin.qq.com/s/ueo9zNMx1OO4cScebORN9Q)

[面试题1](https://mp.weixin.qq.com/s/Z4a8wbWvPDGFTkKJH0X9VQ)

[缓存一致性](https://mp.weixin.qq.com/s/GU3cbUkI84IMwttDz16P3w)

[Redis 持久化策略浅析](https://mp.weixin.qq.com/s/v4z9tUm46mUN4SxxMwwP6A)

[一文搞懂 Redis 架构演化之路](https://mp.weixin.qq.com/s/QssILJLna_v7XQWtV5UMzA)

#### mongo

[B/B+树](https://mp.weixin.qq.com/s/kRG8osOgLIenr7UeEqT7aQ)

[原子性](https://mp.weixin.qq.com/s/GoQg5FFG_5sDBVRF4OqDFA)

[技术从0到1](https://mp.weixin.qq.com/s/FrEqtjMQeQnRvDX6zO1Bhw)

[文件存储](https://mp.weixin.qq.com/s/wXnExtpQAuV9OV3KbWVCwQ)

[优化指南](https://mp.weixin.qq.com/s/fA4Y69Xi7iZPdF8LwBSayg)

[优化指南2](https://mp.weixin.qq.com/s/izRaZ-oKXYAN1RFC8vWCMw)

#### Mysql

[优化原理剖析](https://mp.weixin.qq.com/s/iSSvKqNFSRhcym8X-_A8vQ)

[SQL 查询并不是从 SELECT 开始的](https://mp.weixin.qq.com/s/5BF12rIs1QXQpX4vpKkL0Q)

[mysql技术内幕笔记](https://www.cnblogs.com/BlueMountain-HaggenDazs/category/1252321.html)

[mysql面试题](https://mp.weixin.qq.com/s/b7jLlHpNGB18VwUY_WeDLg)

------

### 消息队列

[Kafka](https://mp.weixin.qq.com/s/piD5ovHonJ6DiQm7fyXJvw)

[面试角度学Kafka](https://mp.weixin.qq.com/s/QF9b9vpncLS24xMzFkanTQ)

[Kafka的存储架构](https://mp.weixin.qq.com/s/p45FtD673s-cdkeHqrEc-g)

[Kafka在美团数据平台的实践](https://mp.weixin.qq.com/s/waVLtusovUkVDt7rKCcdDg)

[rabbitmq](https://mp.weixin.qq.com/s/qSBaD1MInJrvl23kOeeMeA)

[延时队列](https://mp.weixin.qq.com/s/qGywX7S8P3toy-RhQonDYQ)

[复习精讲](https://mp.weixin.qq.com/s/rzEX0wQCoDBxuFmws9f7Lw)

[消息投递](https://mp.weixin.qq.com/s/-jb-FAXzUVepTLFpmgZt8A)

[消息幂等](https://mp.weixin.qq.com/s/E5jtwOhiDzpydr_Leot3RA)

[消息队列选型分析](https://mp.weixin.qq.com/s/6PcvA-8Kfb1LsFKN-ksZkA)

[设计难题](https://mp.weixin.qq.com/s/C1tgYwiBoRJY3A7_WAP20w)

[写个消息中间件](https://mp.weixin.qq.com/s?__biz=MzkxNTE3NjQ3MA==&mid=2247485721&idx=1&sn=a30a9be1685d88c61d7dc5722d50d9c3&source=41#wechat_redirect)

[面试连环问](https://mp.weixin.qq.com/s?__biz=MzkxNTE3NjQ3MA==&mid=2247485753&idx=1&sn=d22f8adc8eb0dfc08163e160127f6b17&source=41#wechat_redirect)

[解决消息队列的数据积压问题](https://mp.weixin.qq.com/s/-DjqcjHxDVUfIC4hf_BkiA)

[消息队列背后的设计思想](https://mp.weixin.qq.com/s/k8sA6XPrp80JiNbuwKaVfg)

[消息队列基本原理和选型对比](https://mp.weixin.qq.com/s/_oO-EZXZq8kUWxvJpdOGDA)

------

### ElasticSearch

[入门](https://mp.weixin.qq.com/s/gHTLSB1sBOlrJ3F8U9affQ)

[入门2](https://mp.weixin.qq.com/s/l20pmtgwuBUMv6JUdzXIbg)

[原来 Elasticsearch 还可以这么理解](https://mp.weixin.qq.com/s/DRQt_r1ZqECO07IsJKClbA)

[美团外卖搜索基于Elasticsearch的优化实践](https://mp.weixin.qq.com/s/6k8THshasaYfSaLr58O1NA)

[常见错误及最佳实践](https://mp.weixin.qq.com/s/zsAk7clgxzrjWLpQbYoTXg)

[优化实战](https://mp.weixin.qq.com/s/PFzRT5Ky0reMXrMRJsj2jQ)

[优化实战2](https://mp.weixin.qq.com/s?__biz=MzA3ODIxNjYxNQ==&mid=2247487186&amp;idx=1&amp;sn=f64ab0c1597b6ae55b0b15229808f413&source=41&key=&ascene=14&uin=&devicetype=Windows+10&version=620603c8&lang=zh_CN&winzoom=1)

------

### prometheus 

[深入理解prometheus](https://mp.weixin.qq.com/s/AjN6fq5DPs4QQhZ0Lc4eDQ)


### 分布式任务
[如何做好分布式任务调度](https://mp.weixin.qq.com/s/xdJzwaNfPGE0utV0gNBb6A)


### 分布式唯一 ID 生成方案浅谈
[如何做好分布式任务调度](https://mp.weixin.qq.com/s/10hn22MInanJXuT6wOYh1Q)

------

### 微服务

[api 设计](https://mp.weixin.qq.com/s/IMXHaibmiskOBwZlk3wpiA)

[为什么我使用 GraphQL 而放弃 REST API](https://mp.weixin.qq.com/s/n1HGGe4_Ty8q7sMbORCADg)

[Spring GraphQL](https://mp.weixin.qq.com/s/4YFnVUGmNm79PQ-stGHs2g)

#### OAuth

[OAuth2](https://mp.weixin.qq.com/s/XhOfr8aYfUYLW0VRCB1PmQ)

[第三方账号登陆 ](https://mp.weixin.qq.com/s/N_Dz4R4tyUpoeQskUEyarg)

------

### 数据结构

[红黑树](https://mp.weixin.qq.com/s/gaOGm48mnONtV4wEE4uVCA)

[红黑树图解](https://mp.weixin.qq.com/s/kEaqW0FgzkU0X6UUQBm0-w)

[跳跃表](https://mp.weixin.qq.com/s/XY1gPvdV7hWTDYNDDW2zoQ)

------

### 高可用

[高性能](https://mp.weixin.qq.com/s/gsHiRnWdYNXnX4ycsRSAWA)

[熔断](https://mp.weixin.qq.com/s/n9wpL6uSjza2nEprLbJDKw)

[熔断原理](https://mp.weixin.qq.com/s/4JLDjEVoYnceKcbBH4zm5w)

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

[一文搞懂一致性hash的原理和实现](https://mp.weixin.qq.com/s/dpwC4TAAO1CdlPWIC_KFUg)

------

### 加密

[常见加密算法](https://mp.weixin.qq.com/s/x_y6w-F1lCN102E8KQmuvQ)

------

### 设计模式

[go设计模式代码实现](http://lailin.xyz/post/singleton.html)

[go设计模式](https://mp.weixin.qq.com/s/VZfwNlqSLzCK0hWSfG4Yzw)

[图解9种常见设计模式](https://mp.weixin.qq.com/s/-jpIitC1j3geciJzkuexdA)

[23 种设计模式的通俗解释，虽然有点污，但是秒懂](https://mp.weixin.qq.com/s/3CzHf8sDz_AjxDTROfuyTA)

[图文详解 23 种设计模式](https://mp.weixin.qq.com/s/MYnCbyhiAClg9Q0IEp6kVA)

[谈谈我工作中的23个设计模式](https://mp.weixin.qq.com/s/kc7tgGLiPUrmq67da9Uhow)

[工厂模式](https://mp.weixin.qq.com/s/jnKIcqNgtzgP-N5ut1J5CA)

[观察者模式](https://mp.weixin.qq.com/s/zT4d2snbG8td8fg9Gt--ig)

[模板模式](https://mp.weixin.qq.com/s/SUpG6A5UAn8gGa2BWFb1ZA)

[策略模式](https://mp.weixin.qq.com/s/mRuDqT7H-zFbrkI9bw5IdA)

[建造者模式](https://mp.weixin.qq.com/s/6Np5C9qUCqDKZZNXGzCc2w)

[通俗解释](https://mp.weixin.qq.com/s/3nhrHU84FNNulKYzHAyETA)

[mybatis中的9种](https://mp.weixin.qq.com/s/d_2Pom9BfgTHbQf2h8O0LA)

------

### 代码质量

[如何提高代码的可读性](https://mp.weixin.qq.com/s/_fg_oS74DEd4jKqJFHKHzg)

------

### 学习之路

- Go：https://github.com/Alikhll/golang-developer-roadmap
- React：https://github.com/adam-golab/react-developer-roadmap
- Rust Web：https://github.com/anshulrgoyal/rust-web-developer-roadmap
- ASP.NET：https://github.com/MoienTajik/AspNetCore-Developer-Roadmap
- Java：https://github.com/s4kibs4mi/java-developer-roadmap
- Flutter：https://github.com/DroidsOnRoids/flutter-roadmap
- NLP：https://github.com/graykode/nlp-roadmap

------

### 一致性

[一致性哈希](https://mp.weixin.qq.com/s/Q9MaeHXk6PPTOGfSFclURQ)

[深入理解完美哈希](https://mp.weixin.qq.com/s/M8Wcj8sZ7UF1CMr887Puog)

[面试1](https://mp.weixin.qq.com/s/VNr6pOygrzICXUi2YXRchA)

------

### 锁

[乐观锁与悲观锁](https://mp.weixin.qq.com/s/XO_mw76JoPUJP7WtKD1mbg)

[聊聊分布式锁](https://mp.weixin.qq.com/s/-N4x6EkxwAYDGdJhwvmZLw)

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

[玩转链路追踪](https://mp.weixin.qq.com/s/xmSar4aG_HVuPvAi6auQOQ)

[GraphQL](https://mp.weixin.qq.com/s?__biz=MzA4Nzc4MjI4MQ==&mid=2652404013&idx=1&sn=a259af0c9cd667ea860801aabb97dbc3&chksm=8bd8ffcbbcaf76dd763a1796928cc0e73f7af5517415c050959358a6c4a4390612abdfea642b&token=2128286661&lang=zh_CN#rd)

[数据中台](https://mp.weixin.qq.com/s/NIG5PfWMwWRpPgQVti3xqA)

[推荐系统](https://mp.weixin.qq.com/s/yQavfvBayYbMEc7c9ObMxg)

[稳定性规范](https://mp.weixin.qq.com/s/gVNKibDQ6UsX_q8_CHvg1A)

[优雅向前兼容](https://mp.weixin.qq.com/s/2PMte2zhaf9tUmMvHiEwxw)

[微服务架构中10个常用的设计模式](https://mp.weixin.qq.com/s/PzPfWHVanSQpZha7qDeKGw)

------

### kubernetes

[入门](http://matt33.com/2020/08/02/kubernetes-start/?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[Kubernetes如果是个水族馆！](https://mp.weixin.qq.com/s/4vHeH3x1lshztODLzR-48Q)

[Kubernetes原理](https://mp.weixin.qq.com/s/nGRUBlW0JnEDZXQaoEDjRg)

[对象](https://mp.weixin.qq.com/s/qrJ50ma4LWBuOn_7WPGznw)

[14个Kubernetes必备基础](https://mp.weixin.qq.com/s/vN228a07K5T82pU6Vg0DYQ)

[干货文章100](https://mp.weixin.qq.com/s/8A_It3NNklbbG--P6Dw9gQ)

[pod 入门指南](https://mp.weixin.qq.com/s/igpOZUszs8sNT4_226bnwA)

[pod创建](https://mp.weixin.qq.com/s/lcenZGKTkAcTT7DZrhBbvw)

[带你畅游 Kubernetes 调度器](https://mp.weixin.qq.com/s/jH9ho9bFNEt0UEsnKmifig)

[大白话告诉你到底用不用学习这该死的Kubernetes容器化](https://mp.weixin.qq.com/s/2WOgn_9_5sx9_1uSIWlg8A)

[部署debug](https://donge.org/posts/envoy-vs-traefik/?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[[Envoy VS Traefik](https://donge.org/posts/envoy-vs-traefik/?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

[4 种常用的 Kubernetes 容器](https://mp.weixin.qq.com/s/khJXu3-pHKRXzTxS4dcgJA)

[运维锦囊，19个K8S日常故障处理解决方案](https://mp.weixin.qq.com/s/47RGWBogU5hbkQu5lKhGhA)

[Envoy 几种负责均衡算法](https://mp.weixin.qq.com/s/Yxo4tua34w2O5BDNVtFm2w)

[最佳实践](https://mp.weixin.qq.com/s/CGcwPahTjjrDZZXHy_vKpA)

[最简单的 K8S 部署文件编写姿势，没有之一！](https://mp.weixin.qq.com/s/uwIHQb2Rm8OQ_w9OHIL7hw)

[入门实战](https://mp.weixin.qq.com/s/sq6zq7I1emVzFnSTlQKQRw)

[50个面试问题](https://mp.weixin.qq.com/s/ctFbNctTbQEZixjKblfcyw)

[CI/CD](https://mp.weixin.qq.com/s/E21w94x7iu6BCY7dXF9-WQ)

[工具](https://mp.weixin.qq.com/s/DL2M_Y6ILIwtctm97ZisDA)

------

#### IM

[微信、陌陌等著名IM软件设计架构](https://mp.weixin.qq.com/s/xzvC_C5aq727diKL1SXeZg)

------

#### Istio

[简介](http://jartto.wang/2020/07/29/istio-1/?hmsr=toutiao.io&utm_medium=toutiao.io&utm_source=toutiao.io)

------

### 运维

[CI/CD](https://mp.weixin.qq.com/s/XDMXxM6A-S99Rf26OQH_hg)

[Devops](https://mp.weixin.qq.com/s/NWzUzX6wss7WeuVI_oFuHQ)

[72 个网络应用安全实操要点，全方位保护你的 Web 应用](https://mp.weixin.qq.com/s/hkBu8Lc4eiBA0gsXfiZwhA)

#### 监控

[监控告警](https://mp.weixin.qq.com/s/qaNWBlDGgE2hNnu6SV4EBg)

[监控体系](https://mp.weixin.qq.com/s/FGCZws3bQ9l9zOWDRTfdhg)

[监控工具](https://mp.weixin.qq.com/s/M-ygzU0V8hgITqx0Wdl6iQ)

[prometheus微服务监控](https://mp.weixin.qq.com/s/mbR_VX2G-exNRGKmwqqshA)

[基于 Prometheus、InfluxDB 与 Grafana 打造监控平台](https://mp.weixin.qq.com/s/IC79mZkqTRQa5JsBxGjmKA)

------

### 面试题

[简历与项目介绍](https://mp.weixin.qq.com/s/phLXpzW6Vz7llcWijjmMUg)

[面试归类](https://mp.weixin.qq.com/s/Elq7SWRpH08KmhX7auboOA)

[面试1](https://mp.weixin.qq.com/s/puhJymLO8IqMoHpzXR-d9w)

[面试2](https://mp.weixin.qq.com/s/pA2pYdoZU8ZIZoFm9txESw)

[面试3](https://mp.weixin.qq.com/s/dPDou-DKCYqzTHTHX6A0Bw)

[面试4](https://mp.weixin.qq.com/s/KsBaBGBCjSUB9x_pfDYXPA)

[golang 50问](https://mp.weixin.qq.com/s/gp-4KCc0JcuSA05jXpVYuA)

[八股文](https://mp.weixin.qq.com/s/tKuecP_dSAbldGTKb9-74Q)

