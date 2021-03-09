# Airport-toolkit
各類方便機場主進行安裝維護的shell腳本    
安裝使用指南請參見 [此鏈接](https://wiki.sspanel.host/#/turnkey-install-for-node?id=%e5%90%8e%e7%ab%af%e4%b8%80%e9%94%ae%e5%ae%89%e8%a3%85%e8%84%9a%e6%9c%ac%ef%bc%88%e5%a4%a7%e7%8c%ab%e7%8c%ab%e7%89%88%ef%bc%89)

安装
CentOS 7（非主要支持版本，请有条件的优先使用CentOS 8）

    yum install wget -y && wget https://raw.githubusercontent.com/secondw/Airport-toolkit/master/ssr_node_c7.sh && chmod +x ssr_node_c7.sh && ./ssr_node_c7.sh

CentOS 8

    dnf install wget -y && wget https://raw.githubusercontent.com/secondw/Airport-toolkit/master/ssr_node_c8.sh && chmod +x ssr_node_c8.sh && ./ssr_node_c8.sh

卸载

    systemctl disable ssr_node && \rm /usr/lib/systemd/system/ssr_node.service && \rm -rf /soft/shadowsocks

服务启动

    systemctl start ssr_node

服务停止

    systemctl stop ssr_node
