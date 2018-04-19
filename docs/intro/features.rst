Features
================================
- 注册发现：帮助微服务自注册并发现其他微服务
- 插件化注册中心：默认对接Service Center和文件系统，开发者可自己扩展Kubernetes，Consul，Eureka等服务
- 限流：提供客户端与服务端限流
- 负载均衡：提供Filter与Strategy2种方式对实例进行选择，并可定制
- 熔断：可通过超时时间，错误率，并发量等条件进行熔断控制，保护系统，防止雪崩效应
- 降级：熔断后可配置降级策略
- 处理链：支持在一次请求调用中，插入自己的处理逻辑
- 插件化协议：默认支持http,Highway RPC 2种协议
- 插件化Cipher：在证书，aksk等敏感数据加载时，支持使用自己的加解密算法
- Metrics：支持导出Prometheus格式监控数据
- Tracing：分布式调用链追踪，支持对接Zipkin
- 日志：支持扩展自己的Writer实现，可上报给kafka，Elasticseach等组件，默认支持本地文件和stdout
- 动态配置框架：对接不同Source，当Source中的配置项出现变化，将触发事件，让微服务感知，用户可自定义事件触发的动作
- 配置热加载：负载均衡，熔断，降级等等配置支持运行时热加载