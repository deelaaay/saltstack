# saltstack
该配置环境主要是配置haproxy + keepalived负载均衡的高可用，其中haproxy通过轮训的方式连接到后端实际的2 台nginx服务器.仅供自己学习使用，部署内容参考网络资源，若原作者觉得侵权，联系我，即刻更正。

全部虚拟机操作
主机名  角色     ip
master master 192.168.4.10
minion1 haproxy keepalived 192.168.4.11
minion2 haproxy keepalived 192.168.4.12
minion3 nginx 192.168.4.13
minion3 nginx 192.168.4.14
  VIP 192.168.4.16
