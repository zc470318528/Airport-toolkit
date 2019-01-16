支持系统：CentOS 7 x64 and Ubuntu 18.04 x64 脚本功能：

可选配置节点为WebAPI模式或SQL模式
可选配置单端口多用户
可选启用BBR（from mainline kernel）
可选注册为系统服务
————————————————————————————————————————————————————————————————————————————————————————————————————————————————————
使用指南
————————————————————————————————————————————————————————————————————————————————————————————————————————————————————
安装 For CentOS 7 x64

yum install wget -y && wget https://raw.githubusercontent.com/SuicidalCat/Airport-toolkit/master/ssr_node_c7.sh && chmod +x ssr_node_c7.sh && ./ssr_node_c7.sh
————————————————————————————————————————————————————————————————————————————————————————————————————————————————————
安装 For Ubuntu 18.04 x64

yum install wget -y && wget https://raw.githubusercontent.com/SuicidalCat/Airport-toolkit/master/ssr_node_u18.sh && chmod +x ssr_node_u18.sh && ./ssr_node_u18.sh
————————————————————————————————————————————————————————————————————————————————————————————————————————————————————
卸载
systemctl disable ssr_node && \rm /usr/lib/systemd/system/ssr_node.service && \rm -rf /soft/shadowsocks

设置开机启动
systemctl enable ssr_node

服务启动
systemctl start ssr_node

服务停止
systemctl stop ssr_node
