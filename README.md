# 医药集中采购系统-后台管理

>简介：

## 模块划分
## 1.基础模块
### 1.注册中心
##### springcloud-eureka 注册中心server[sc-eureka:8761、8762、8763]
访问地址：http://localhost:8761/，http://localhost:8762/，http://localhost:8763/
##### springcloud-config 配置中心server[sc-config:8888]
访问地址：
##### springcloud-zuul 配置中心server:[sc-zuul:9999]
访问地址：http://localhost:9999/
##### springcloud-admins 配置中心server:[sc-admins:9001]
访问地址：
##### springcloud-turbine 配置中心server:[sc-turbine:7811]
访问地址：
##### springcloud-zipkin 配置中心server:[sc-zipkin:7911]
访问地址：
>---
## 2.功能模块
### 1.用户模块
##### springcloud-user 用户模块的server:[sc-user:7800]
访问地址：http://localhost:9999/user-api/
##### springcloud-user-api 用户模块的api:[sc-user-api:7890]
访问地址：

### 2.供货商药品目录模块（药品目录模块）
##### springcloud-ypml 用户模块的server:[sc-ypml:7803]
访问地址：http://localhost:9999/ypml-api/
##### springcloud-ypml-api 用户模块的api:[sc-ypml-api:7891]
访问地址：

### 3.采购单模块
##### springcloud-cgd 用户模块的server:[sc-cgd:7804]
访问地址：http://localhost:9999/cgd-api/user
##### springcloud-cgd-api 用户模块的api:[sc-cgd-api:7892]
访问地址：


## 启动顺序
##### 1.sc-eureka 注册中心
##### 2.sc-config 配置中心
##### 3.sc-admins 集群监控
##### 4.sc-zipkin 链路追踪
##### 5.sc-user   模块服务
##### 6.sc-user-api 模块服务api
##### 7.sc-turbine 聚合监控服务
##### 8.sc-zuul   网关服务