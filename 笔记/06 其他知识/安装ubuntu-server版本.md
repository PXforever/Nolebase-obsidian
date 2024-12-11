---
share: "true"
---
> ubuntu版本有：
> + desktop
> + server
> + core
> desktop的是比较通用版本，但是对于低性能设备，响应速度慢。所以如果没有图像需求，则最好使用server。
> core版本是提供IOT设备使用，也就是嵌入式设备使用，这部分因为使用的是`snap`应用，不太适应。

这里使用的是`virtual box`虚拟机进行安装，`ubuntu`版本为：`ubuntu-22.04.4-live-server-amd64.iso`。
# 安装
## 创建OS虚拟机
![[笔记/01 附件/安装ubuntu-server版本/image-20240721100411170.png|笔记/01 附件/安装ubuntu-server版本/image-20240721100411170.png]]
![[笔记/01 附件/安装ubuntu-server版本/image-20240721100512198.png|笔记/01 附件/安装ubuntu-server版本/image-20240721100512198.png]]
![[笔记/01 附件/安装ubuntu-server版本/image-20240721100620301.png|笔记/01 附件/安装ubuntu-server版本/image-20240721100620301.png]]
![[笔记/01 附件/安装ubuntu-server版本/image-20240721100821330.png|笔记/01 附件/安装ubuntu-server版本/image-20240721100821330.png]]

![[笔记/01 附件/安装ubuntu-server版本/image-20240721100909060.png|笔记/01 附件/安装ubuntu-server版本/image-20240721100909060.png]]
## 安装配置
![[笔记/01 附件/安装ubuntu-server版本/image-20240721101016733.png|笔记/01 附件/安装ubuntu-server版本/image-20240721101016733.png]]
提示你有新版本`24.04`，我们不安装
![[笔记/01 附件/安装ubuntu-server版本/image-20240721101037152.png|笔记/01 附件/安装ubuntu-server版本/image-20240721101037152.png]]
键盘选择，美式键盘：
![[笔记/01 附件/安装ubuntu-server版本/image-20240721101131828.png|笔记/01 附件/安装ubuntu-server版本/image-20240721101131828.png]]
我们可以选择最小版本，也可以正常版本：
![[笔记/01 附件/安装ubuntu-server版本/image-20240721101226760.png|笔记/01 附件/安装ubuntu-server版本/image-20240721101226760.png]]
网络配置，我们设置静态网络(建议DHCP，这里因为需要演示一下，因为静态没设置好是没有网络的)：
![[笔记/01 附件/安装ubuntu-server版本/image-20240721101307379.png|笔记/01 附件/安装ubuntu-server版本/image-20240721101307379.png]]
![[笔记/01 附件/安装ubuntu-server版本/image-20240721101323892.png|笔记/01 附件/安装ubuntu-server版本/image-20240721101323892.png]]
![[笔记/01 附件/安装ubuntu-server版本/image-20240721101338352.png|笔记/01 附件/安装ubuntu-server版本/image-20240721101338352.png]]

![[笔记/01 附件/安装ubuntu-server版本/image-20240721101617135.png|笔记/01 附件/安装ubuntu-server版本/image-20240721101617135.png]]
可以设置代理，这里不设置：
![[笔记/01 附件/安装ubuntu-server版本/image-20240721101712759.png|笔记/01 附件/安装ubuntu-server版本/image-20240721101712759.png]]
这里软件源地址，不改动，也可以自己改为国内源：
![[笔记/01 附件/安装ubuntu-server版本/image-20240721101755213.png|笔记/01 附件/安装ubuntu-server版本/image-20240721101755213.png]]
我们可以设置用整个硬盘，不过这里使用自定义划分：
![[笔记/01 附件/安装ubuntu-server版本/image-20240721101855053.png|笔记/01 附件/安装ubuntu-server版本/image-20240721101855053.png]]

![[笔记/01 附件/安装ubuntu-server版本/image-20240721101917995.png|笔记/01 附件/安装ubuntu-server版本/image-20240721101917995.png]]
创建`boot`分区：
![[笔记/01 附件/安装ubuntu-server版本/image-20240721102027049.png|笔记/01 附件/安装ubuntu-server版本/image-20240721102027049.png]]
![[笔记/01 附件/安装ubuntu-server版本/image-20240721102046951.png|笔记/01 附件/安装ubuntu-server版本/image-20240721102046951.png]]
创建交换分区：
![[笔记/01 附件/安装ubuntu-server版本/image-20240721102257375.png|笔记/01 附件/安装ubuntu-server版本/image-20240721102257375.png]]
创建文件系统，这里不填容量，表示使用全部：
![[笔记/01 附件/安装ubuntu-server版本/image-20240721102153052.png|笔记/01 附件/安装ubuntu-server版本/image-20240721102153052.png]]
![[笔记/01 附件/安装ubuntu-server版本/image-20240721102326789.png|笔记/01 附件/安装ubuntu-server版本/image-20240721102326789.png]]
![[笔记/01 附件/安装ubuntu-server版本/image-20240721102350460.png|笔记/01 附件/安装ubuntu-server版本/image-20240721102350460.png]]
警告你确定后就没办法返回上面的页面了，我们继续。
![[笔记/01 附件/安装ubuntu-server版本/image-20240721102543951.png|笔记/01 附件/安装ubuntu-server版本/image-20240721102543951.png]]
![[笔记/01 附件/安装ubuntu-server版本/image-20240721102609865.png|笔记/01 附件/安装ubuntu-server版本/image-20240721102609865.png]]
![[笔记/01 附件/安装ubuntu-server版本/image-20240721102641201.png|笔记/01 附件/安装ubuntu-server版本/image-20240721102641201.png]]
等待完成安装：
![[笔记/01 附件/安装ubuntu-server版本/image-20240721102705738.png|笔记/01 附件/安装ubuntu-server版本/image-20240721102705738.png]]
重启：
![[笔记/01 附件/安装ubuntu-server版本/image-20240721102903774.png|笔记/01 附件/安装ubuntu-server版本/image-20240721102903774.png]]
到这里已经完成安装了,我们再添加一下网卡：
![[笔记/01 附件/安装ubuntu-server版本/image-20240721103911497.png|笔记/01 附件/安装ubuntu-server版本/image-20240721103911497.png]]
# 预装软件建议：
![[笔记/01 附件/安装ubuntu-server版本/image-20240721103200604.png|笔记/01 附件/安装ubuntu-server版本/image-20240721103200604.png]]
我们使用`sudo apt install`按照如下软件：
```shell
sudo apt update
sudo apt install vim  parted gparted net-tools iputils-ping samba gdb make gcc
```
安装后，如果设置静态网络没有网络，我们想设置为动态的话：
```shell
echo -e "network:\n\tversion: 2\n\tethernets:\n\t\tenp0s3:\n\t\t\tdhcp4:true" > /etc/netplan/00-xxxxx.ymal
```























