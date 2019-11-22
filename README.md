# Linux-NetSpeed

wget: command not found的解决方法:yum -y install wget 回车即可

bash: curl: command not found的解决方法:apt-get install curl  回车即可

魔改版bbr加速：wget -N --no-check-certificate "https://raw.githubusercontent.com/wangxiaoke123/Linux-NetSpeed/master/tcp.sh" && chmod +x tcp.sh && ./tcp.sh

查看状态 ./tcp.sh

需要按8，进行系统优化

回程路由：wget https://raw.githubusercontent.com/nanqinlang-script/testrace/master/testrace.sh

bash testrace.sh

硬件信息：
wget -qO- --no-check-certificate https://raw.githubusercontent.com/oooldking/script/master/superbench.sh | bash

服务器测速代码 

curl -s https://raw.githubusercontent.com/sivel/speedtest-cli/master/speedtest.py | python -
