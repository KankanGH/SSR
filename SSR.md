### SSR
This Process is only for SSR Set-up
#
### End Firewall
`/etc/init.d/iptables stop` / If not, the VPS will not allow remote connections.
# 
### SSR Installation
`wget --no-check-certificate https://freed.ga/github/shadowsocksR.sh; bash shadowsocksR.sh`
#
### ServerSpeeder Installation
```
uname -r
rpm -ivh https://freed.ga/kernel/kernel-firmware-2.6.32-504.3.3.el6.noarch.rpm
rpm -ivh https://freed.ga/kernel/kernel-2.6.32-504.3.3.el6.x86_64.rpm --force
reboot
wget -N --no-check-certificate https://raw.githubusercontent.com/Adair-Hsu/SSR/master/SpeederInstall.sh && bash SpeederInstall.sh
```
### Alternate Address for ServerSpeeder Installation
`https://raw.githubusercontent.com/91yun/serverspeeder/master/serverspeeder-all.sh`
