# mecroservice-eureka


```$xslt 
创建网卡  microservice-network
docker network create -d bridge microservice-network

容器启动命令
docker run -p 7000:7000 --name microservice-eureka --network microservice-network -m 50M --cpus=0.05  -d registry.cn-hangzhou.aliyuncs.com/match-hub/microservice-eureka:1.0

docker run -p 7000:7000 --name microservice-eureka --network microservice-network -m 50M --cpus=0.05  -d registry.cn-hangzhou.aliyuncs.com/match-hub/microservice-eureka:1.0


在其他容器访问当前容器 
curl http://microservice-eureka
ping   microservice-eureka
```