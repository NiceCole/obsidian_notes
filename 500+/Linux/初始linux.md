1，配备linux所需要的环境 vmware
2，linux安装需要注意的点：
	1）硬件选择 n核nG
	2）安装的时候需要使用镜像源 百度上找一个即可
	3）linux的连接 
		比如连接阿里云的服务器 需要再服务器上面设置好对应的ssh密钥 本地才能连接到对应的阿里云服务区
3，linux初始化进程之systemd
	1）systemctl start sn.service 用来启动一个服务（并不会重启现有的）
	2）systemctl stop sn.service 用来停止一个服务（并不会重启现有的）
	3）systemctl restart sn.service 用来停止并启动一个服务 
	4）systemctl reload sn.service 重新装在配置文件而不中断服务
	5）systemctl status sn.service 汇报服务是否正在运行
	6）systemctl status firewalld.service 查看系统防火墙服务的状态
	7）systemctl stop firewalld.service 停止系统防火墙服务的状态
	8）systemctl disable firewalld.service 设置系统防火墙不开机自启动