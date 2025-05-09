##### OpenWrt初始化
```
curl -# -o /etc/crontabs/root https://raw.githubusercontent.com/tieguangfeng/openwrt/refs/heads/main/crontabs.txt
curl -# -o /etc/myhosts https://raw.githubusercontent.com/tieguangfeng/openwrt/refs/heads/main/myhosts
curl -# -o /etc/homeproxy/resources/proxy_list.txt https://raw.githubusercontent.com/tieguangfeng/openwrt/refs/heads/main/homeproxy/proxy_list.txt
curl -# -o /etc/homeproxy/resources/direct_list.txt https://raw.githubusercontent.com/tieguangfeng/openwrt/refs/heads/main/homeproxy/direct_list.txt
```
##### 系统重置
```
rm -rvf /overlay/*  
```
crontabs.txt[定时重启]  
proxy_list.txt[代理域名]  
direct_list.txt[直连域名]  
myhosts[广告过滤]  
##### 代理端口
22,53,80,443,465,853,873,995,5222,8080,8443,9418  
