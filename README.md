# survey

serveless调研

## 产品罗列：

### 商业化产品：
- awk lambda
- azure function
- tecent serverless cloud function
- google cloud function
- huawei function graph

### 开源产品：

- funktion
- serverless framework
- openfaas
- fn project
- openwhisk
- fission
- nuclio
- shipwright
- cloud native buildpacks
- keda
- dapr
- openfunction
- knative
- kubeless
- serverless

## 测评维度：

1.安装部署运维
2.整体资源占用
3.底层技术
4.文档
5.开发语言
6.打包机制
7.github人气
8.架构图
9.代码存储
10.函数/应用构建流程 (cicd)

## serverless使用场景

来源：https://www2.eecs.berkeley.edu/Pubs/TechRpts/2019/EECS-2019-3.pdf

| 百分比 | 场景                                                         |
| ------ | ------------------------------------------------------------ |
| 32%    | Web and API serving                                          |
| 21%    | Data Processing, e.g., batch ETL (database Extract, Transform, and Load) |
| 17%    | Integrating 3rd Party Services                               |
| 16%    | Internal tooling                                             |
| 8%     | Chat bots e.g., Alexa Skills (SDK for Alexa AI Assistant)    |
| 6%     | Internet of Things                                           |


## serverless价值
* 节省长尾应用的使用资源
* 节省开发运维成本 (如果认为serverless应用包含微服务应用和函数式应用，那么可以用一个平台负责所有业务监控日志自动扩缩容)
* 

## 关键设计点

### 镜像分发
* 懒加载
* p2p镜像加速

### 调度


### faas落地灵魂3问
* 存量业务改造
* faas碎片化问题
* 研发提效问题

来源：[1688 复杂业务场景下的 Serverless 提效实践](https://developer.aliyun.com/article/874568?spm=a2c6h.12873639.0.0.771745ffHl9QnW)

### serverless原生心智
1. 我的业务是什么？
2. 做这件事情能不能让我的业务出类拔萃？
3. 如果不能，我为什么要做这件事情而不是让别人来解决这个问题？
4. 在解决业务问题之前没有必要解决技术问题

> 在实践 Serverless 架构时，最重要的心智不是选择哪些流行服务和技术，攻克哪些技术难题，而是时刻铭记在心专注业务逻辑，这样更容易让我们选择合适的技术和服务，明确如何设计应用架构。

![img](https://ucc.alicdn.com/images/lark/0/2021/png/22456429/1633941947549-358cbb19-8ac9-4f85-9a6d-56b2f42e2148.png)

来源：[Serverless 架构模式及演进](https://developer.aliyun.com/article/799135)

## 参考资料：

* [Cloud Programming Simplified: A Berkeley View on Serverless Computing](https://www2.eecs.berkeley.edu/Pubs/TechRpts/2019/EECS-2019-3.pdf)
* [serverless 开源框架对比](https://bbs.huaweicloud.com/blogs/247064)
* [Serverless Open-Source Frameworks: OpenFaaS, Knative, & more](https://www.cncf.io/blog/2020/04/13/serverless-open-source-frameworks-openfaas-knative-more/)
* [Serverless 架构模式及演进](https://developer.aliyun.com/article/799135)
* [Serverless 背景下的前端困境与解决方案](https://developer.aliyun.com/article/726945)
* 

### 微信公众号码农架构
* [通过一个Serverless案例，理解FaaS的运行逻辑](https://mp.weixin.qq.com/s?__biz=MzU3OTc1MDM1Mg==&mid=2247488873&idx=1&sn=a4e057de9f033f164247c549a8ce0f41&chksm=fd6005d6ca178cc0805bad329acfef864b1d3a39713d1e0cb6d48f0798062772ab789fb129cd&scene=178&cur_album_id=1519689351817904130#rd)
* [深入浅出FaaS的两种进程模型](https://mp.weixin.qq.com/s?__biz=MzU3OTc1MDM1Mg==&mid=2247488942&idx=1&sn=151cf4bf16938d8e4fa4fcb4a51c542f&chksm=fd600511ca178c075e0e7ffed228fe98d3fb521310e859f324d97cad06bbdaad9cf76984408c&scene=178&cur_album_id=1519689351817904130#rd)

收费模型：

1. 函数执行时常
2. 调用次数

进程模型：

1. 用完即毁
2. 常驻

* [深入浅出FaaS应用场景之数据编排](https://mp.weixin.qq.com/s?__biz=MzU3OTc1MDM1Mg==&mid=2247488989&idx=1&sn=e29387863da9bcfb3b14156e2039afe6&chksm=fd600562ca178c747287c429a73104c0a2289f7bd5374d3c9d4e23fb3da016664defe50cdf6a&scene=178&cur_album_id=1519689351817904130#rd)
* [如何将后端BaaS化：NoOps的微服务](https://mp.weixin.qq.com/s?__biz=MzU3OTc1MDM1Mg==&mid=2247489068&idx=2&sn=7e6db18d21ecf47511b2c7d4fe55c09a&chksm=fd600693ca178f85806b8e67ebff61cd4647f1702c215e1dc8ea3fccb75496ed88f6bb80d47a&scene=178&cur_album_id=1519689351817904130#rd)
* [如何将后端BaaS化：业务逻辑的拆与合](https://mp.weixin.qq.com/s?__biz=MzU3OTc1MDM1Mg==&mid=2247489116&idx=1&sn=05c1a6a39a109a19af50c7e729ff821a&chksm=fd6006e3ca178ff56dbcc7a1a14d8d597fb3e8ada2c61fb4189782424713d3a6efb4a04a65cd&scene=178&cur_album_id=1519689351817904130#rd)

### open function相关

* [OpenFunction：新一代开源 FaaS 平台](https://www.infoq.cn/article/aqZsasOwiFAYwvGMkU9O)

### 阿里云相关：

* [如何落地一个FaaS平台？](https://developer.aliyun.com/article/769727?spm=a2c6h.14164896.0.0.37a370a9j1AiRj)
* [阿里云 FaaS 架构设计](https://developer.aliyun.com/article/819594?utm_content=m_1000311816)
* [1688 复杂业务场景下的 Serverless 提效实践](https://developer.aliyun.com/article/874568?spm=a2c6h.12873639.0.0.771745ffHl9QnW)

### 字节跳动相关
* [GMTC 2021 演讲 《字节跳动基于 Serverless 的前端研发模式升级》](https://www.shangyexinzhi.com/article/4005226.html) 基于 Serverless 打造一站式前端解决方案 / garfish前端微服务框架
* [BaaS、FaaS、Serverless都是什么馅儿？](https://cloud.tencent.com/developer/article/1145319)

### 美团相关

* [美团Serverless平台Nest的探索与实践](https://tech.meituan.com/2021/04/21/nest-serverless.html)

1. 演进路线: 先建设FaaS函数计算服务，再建设面向应用的Serverless服务
2. 基础设施: k8s
3. 开发语言: java

创新点：

1. sandbox合并部署,同一个pod内存在多个sandbox,此时将pod抽象为node角色,sandbox抽象为pod角色

### 京东云相关
* [Serverless架构设计与落地应用](https://developer.jdcloud.com/article/979) (公开课视频形式)

### 沙箱sandbox相关
* [基于容器化技术的一个沙箱](https://criyle.github.io/2020/04/29/go-judge/)
* 