# sc-kill

● 该项目是基于SpringCloud, SpringBoot, Mybatis实现的分布式商品秒杀系统， 服务注册中心：eureka。 网关：zuul, 实现熔断，降级，服务负载均衡。使用jmeter进行压测， 开发环境： IDEA ， 数据库： MySQL， 缓存： Redis 。使用Redisson实现分布式锁，令牌桶限流， 雪花算法生成分布式全局唯一订单号。
 使用RabbitMQ削峰，异步生成订单， SpringSession解决分布式Session一致性问题， 解决了超卖，缓存穿透，雪崩等问题。
