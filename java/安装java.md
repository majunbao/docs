Linux 安装配置JDK8环境
https://blog.51cto.com/u_11061155/5661280


UTM安装Centos7

Centos7 安装后没有网络
编辑网络配置：vi /etc/sysconfig/network-scripts/ifcfg-xxx，替换成实际的网卡名。
编辑ONBOOT=no 改成 ONBOOT=yes
执行 systemctl restart network 重启网络
ping qq.com 尝试是否连通

utm linux 开启复制(不行，最终使用mac ssh远程连接)	
安装来宾工具
sudo yum install spice-vdagent
https://docs.getutm.app/guest-support/linux/#fedora-centos-rpm-based

打开ssh，开放22端口
iptables -I INPUT -p tcp --dport 8082 -j ACCEPT

安装mysql-8.0.13
在 /usr/local/ 下执行，下载资源包
wget https://downloads.mysql.com/archives/get/p/23/file/mysql-8.0.21-linux-glibc2.12-x86_64.tar.xz
参考
Contos7 安装 mysql 8 https://www.cnblogs.com/secretmrj/p/15600144.html
数据库密码 mysql123

CentOS: 开放80、22、3306端口操作 https://blog.51cto.com/u_15462264/4865319
iptables规则的查看、添加、插入、删除和修改
https://blog.csdn.net/deeplearnings/article/details/77369297


JAVA 教程
https://www.bilibili.com/video/BV1w64y1r7YP/?p=4&vd_source=16368f5f9e30dd9700a3d31419d995e7
