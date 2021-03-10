# sc-kill

● 该项目是基于SpringCloud, SpringBoot, Mybatis实现的分布式商品秒杀系统， 服务注册中心：eureka。 网关：zuul, 实现熔断，降级，服务负载均衡。使用jmeter进行压测， 开发环境： IDEA ， 数据库： MySQL， 缓存： Redis 。使用Redisson实现分布式锁，令牌桶限流， 雪花算法生成分布式全局唯一订单号。
 使用RabbitMQ削峰，异步生成订单， SpringSession解决分布式Session一致性问题， 解决了超卖，缓存穿透，雪崩等问题。


运行要求： 需启动Redis(6379), Mysql(3306), RabbitMQ(5672). 然后先启动服务注册中心Eureka, 再启动Gateway，两个kill服务。


运行： 

![运行](https://user-images.githubusercontent.com/67009639/110569388-67fef280-818f-11eb-958c-f4b8bc074a48.png)

![结果](https://user-images.githubusercontent.com/67009639/110569422-76e5a500-818f-11eb-839c-f512084b78e6.png)

![结果2](https://user-images.githubusercontent.com/67009639/110569599-ac8a8e00-818f-11eb-989f-e850f3995078.png)

![运行2](https://user-images.githubusercontent.com/67009639/110569433-79e09580-818f-11eb-802e-0c152d93d70c.png)
