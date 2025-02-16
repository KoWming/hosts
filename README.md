# hosts  

## Note  
每日自动更新 github, docker 和 tmdb 的 IP 地址。  

hosts Url:   
Raw Url: https://raw.githubusercontent.com/kekylin/hosts/main/hosts  

## Used  
Windows/MacOS:  
```
推荐使用 SwitchHosts, 官网查看：https://swh.app/zh
```
Linux:
```
# 删除
sudo sed -i '/# Kekylin Hosts Start/,/# Kekylin Hosts End/d' /etc/hosts
# 添加
curl -s -k -L https://raw.githubusercontent.com/kekylin/hosts/main/hosts | sudo tee -a /etc/hosts
# 重启网络
/etc/init.d/network restart
```
