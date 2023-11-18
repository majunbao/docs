yum 是包管理器，内部使用rpm安装软件。yum会自动安装依赖，rpm不会自动按装，但是会给出依赖列表。

安装软件： yum install <package_name>
更新软件： yum update <package_name>
查找软件： yum search <package_name>
删除软件： yum remove <package_name>

安装 ifconfig
鼓励使用 ip 命令，例如查看IP命令：ip address show，如果想要老的命令如ifconfig，使用命令安装 yum install net-tools。

Howto install ifconfig on CentOS 7 Linux
https://linuxconfig.org/howto-install-ifconfig-on-centos-7-linux