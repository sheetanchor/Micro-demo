Eureka  
一个RESTful服务，用来定位运行在AWS地区（Region）中的中间层服务。由两个组件组成：Eureka服务器和Eureka客户端。Eureka服务器用作服务注册服务器。Eureka客户端是一个java客户端，用来简化与服务器的交互、作为轮询负载均衡器，并提供服务的故障切换支持。Netflix在其生产环境中使用的是另外的客户端，它提供基于流量、资源利用率以及出错状态的加权负载均衡。


eureka-server作为服务发现的核心，第一个搭建，后面的服务都要注册到eureka-server上，意思是告诉eureka-server自己的服务地址是啥。当然还可以用zookeeper或者springconsul。

验证地址：
http://localhost:8761/