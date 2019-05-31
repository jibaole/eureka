Eureka
=====
[![Build Status](https://netflixoss.ci.cloudbees.com/job/NetflixOSS/job/eureka/job/eureka-snapshot/badge/icon)](https://netflixoss.ci.cloudbees.com/job/NetflixOSS/job/eureka/job/eureka-snapshot/)

Eureka是一个基于REST(具象状态传输)的服务，主要用于AWS云中定位服务，以实现中间层服务器的负载平衡和故障转移。
在Netflix, Eureka除了在中间层负载平衡中扮演重要角色外，还用于以下目的。

* 帮助Netflix Asgard -一个开源服务，使云部署更容易，在
        +快速回滚版本，以防问题，避免重新启动100个实例，这可能需要很长时间。
        +在滚动推送中，避免在出现问题时将新版本传播到所有实例。

* 或者我们的cassandra部署，从通信流中取出实例进行维护。

* 来标识环中的节点列表。

* 用于由于各种其他原因携带其他特定于应用程序的关于服务的其他特定元数据。


构建
----------
构建需要java8，因为一些必需的库是java8 (servo)，但是源和目标兼容性仍然设置为1.7。

支持
----------
[Eureka Google Group](https://groups.google.com/forum/?fromgroups#!forum/eureka_netflix)


文档
--------------
请看 [wiki](https://github.com/Netflix/eureka/wiki) 的详细文档.


源码入口:
---------------
地址:<https://segmentfault.com/a/1190000011668299>

调试环境搭建
---------------
地址:<https://blog.csdn.net/cyq12345_/article/details/78791291>