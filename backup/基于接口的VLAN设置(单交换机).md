# <center style="color:red；">基于接口的VLAN设置(单交换机)</center>

实验用设备：4个PC机、1个交换机、1个路由器。

拓扑结构：

## 1.配置的拓扑结构图如下：

![网络图片](https://github.com/fengshengbanxia/fengshengbanxia.github.io/raw/main/images/1.png)

## 2.配置主机PC_3，PC_4，PC_5，PC_6

| ![图片 1](https://github.com/fengshengbanxia/fengshengbanxia.github.io/raw/main/images/图片2.png) |![图片 2](https://github.com/fengshengbanxia/fengshengbanxia.github.io/raw/main/images/图片3.png) |
| ----------------------- | ----------------------- |
| ![图片 3](https://github.com/fengshengbanxia/fengshengbanxia.github.io/raw/main/images/图片4.png) | ![图片 4](https://github.com/fengshengbanxia/fengshengbanxia.github.io/raw/main/images/图片5.png)|
| ----------------------- | ----------------------- |

## 3.路由器网关设置（ip：192.168.1.254）和DHCP服务器设置（IP范围：192.168.1.100-192.168.1.200）
设置命令如下：

![图片6](https://github.com/fengshengbanxia/fengshengbanxia.github.io/raw/main/images/图片6.png)

## 4.交换机VLAN设置：VLAN 10 设置接口范围：g1/0/1-g1/0/10
  VLAN 20 设置接口范围：g1/0/20-g1/0/30
---
设置命令如下：
![图片7](https://github.com/fengshengbanxia/fengshengbanxia.github.io/raw/main/images/图片7.png)
![图片8](https://github.com/fengshengbanxia/fengshengbanxia.github.io/raw/main/images/图片8.png)

## 5.自动分配IP地址结果：PC_3，PC_4，PC_5，PC_6
| ![图片 9](https://github.com/fengshengbanxia/fengshengbanxia.github.io/raw/main/images/图片9.png) |![图片 10](https://github.com/fengshengbanxia/fengshengbanxia.github.io/raw/main/images/图片10.png) |
| ----------------------- | ----------------------- |
| ![图片 11](https://github.com/fengshengbanxia/fengshengbanxia.github.io/raw/main/images/图片11.png) | ![图片 12](https://github.com/fengshengbanxia/fengshengbanxia.github.io/raw/main/images/图片12.png)|
| ----------------------- | ----------------------- |
## 6.测试连通性

PC_3 ping PC_4
![图片13](https://github.com/fengshengbanxia/fengshengbanxia.github.io/raw/main/images/图片13.png)
PC_3ping PC_5,PC_3 ping PC_6
![图片14](https://github.com/fengshengbanxia/fengshengbanxia.github.io/raw/main/images/图片14.png)
全部可ping通，实验成功
