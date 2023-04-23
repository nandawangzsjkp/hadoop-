# hadoop-
一点笔记
services.msc

vi /etc/sysconfig/network-scripts/ifcfg-ens33

BOOTPROTO=static

ONBOOT=yes

IPADDR=192.168.80.131
GATEWAY=192.168.80.2
NETMASK=255.255.255.0
DNS1=8.8.8.8

ifconfig

systemctl restart network #重启网卡

vi /etc/hosts #配置一下

reboot #重启

hostnamectl set-hostname+主机名

hostnamectl set-hostname Master

hostname #查看一下

ls

ping www.baidu.com #检查网络是否通

安装yum

mv /etc/yum.repos.d/CentOS-Base.repo /etc/yum.repos.d/CentOS-Base.repo.backup

wget -o /etc/yum.repos.d/CentOS-Base.repo http://mirrors.aliyun.com/repo/Centos-7.repo

wget -O /etc/yum.repos.d/epel.repo http://mirrors.aliyun.com/repo/epel-7.repo

yum clean all#清理缓存

yum makecache#新缓存

rz#验证

