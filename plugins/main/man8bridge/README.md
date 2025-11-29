# Man8Bridge

Man8Bridge的功能如下：
- 主机侧网桥功能相同，默认行为正常桥接
- 默认提供IPv4 masq NAT，使用nftables backend，不使用Vlan。
- 独特功能：（创建主机侧网桥时）根据主机中ygg子网为主机网桥分配全局唯一的ygg子网网关地址
- 独特功能：在创建完容器内网络之后，自动分配容器内ygg子网地址和默认路由