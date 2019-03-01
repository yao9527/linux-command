# linux常用命令大全

## 系统
|作用|命令|
|:-:|:-:|
|查看系统信息|cat /proc/version|

## 常用命令
|作用|命令|操作步骤|
|:-:|:-:|:-:|
|查看端口号被哪个占用|lsof -i:端口号|
|给文件添加删除权限|chattr +i|
|搜索git|find / -name git|
|模糊搜索文件|find . -name "*.conf" \| xargs grep ""|
|查看端口情况|netstat -pan \| grep 80|
|显示当前文件夹文件的个数|ls \| wc -l|
|安装crontab|yum -y install vixie-cron、yum -y install crontabs|
|修改默认22远程端口|vi /etc/ssh/sshd-config|在最末尾添加port端口、重启sshd服务、service sshd restart|
|查看应用安装路径|whereis 文件名称|
|重启nginx|/usr/local/nginx/sbin/nginx -c /usr/local/nginx/conf/nginx.conf|
|快速重启nginx|nginx -s stop|
|完整有序的停止nginx|nginx -s quit|
|查看所有当前tcp端口使用情况|netstat -ntlp|
|查看80端口使用情况|netstat -tpln|grep 80|
|使用代理查看某地址是否能访问|wget http://127.0.0.1/api/crawler/data/filelist -e use_proxy=yes -e http_proxy=代理ip:8002|
|查看某服务的端口|telnet 127.0.0.1 80|
|挂载执行某个python代码|nohup /usr/sbin/python3 /home/cli/a.py &|

