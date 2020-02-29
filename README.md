# Linux-NetSpeed

wget: command not found的解决方法:yum -y install wget 回车即可

如果提示 curl: command not found ，那是因为你的 VPS 没装 Curl

ubuntu/debian 系统安装 Curl 方法: apt-get update -y && apt-get install curl -y

centos 系统安装 Curl 方法: yum update -y && yum install curl -y

魔改版bbr加速：wget -N --no-check-certificate "https://raw.githubusercontent.com/wangxiaoke123/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh

bbrplus加速：wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh

查看状态 ./tcp.sh

需要按8，进行系统优化

执行  lsmod | grep bbr ，以检测 BBR 是否开启

回程路由：wget https://raw.githubusercontent.com/nanqinlang-script/testrace/master/testrace.sh

bash testrace.sh

硬件信息：
wget -qO- --no-check-certificate https://raw.githubusercontent.com/oooldking/script/master/superbench.sh | bash

服务器测速代码 

curl -s https://raw.githubusercontent.com/sivel/speedtest-cli/master/speedtest.py | python -

查看端口是否被占用lsof -i:53

杀掉进程，查看端口对应的pid，例如为792 然后 kill -9 792

查看端口是否开启 
netstat -nupl (UDP类型的端口)
netstat -ntpl (TCP类型的端口)
