## SSR [only works on the system of CentOS (Linux)]
This Process is only for SSR Set-up
#
### End Firewall
`/etc/init.d/iptables stop`
#### Or Firstly:
`service iptables restart`
#### Secondly:
`service iptables stop`
#### If not, the VPS will not allow the remote connections.
# 
### SSR Installation
`wget --no-check-certificate https://freed.ga/github/shadowsocksR.sh; bash shadowsocksR.sh`
#
### ServerSpeeder Installation
#### CentOS 6
```
1. uname -r
2. rpm -ivh https://freed.ga/kernel/kernel-firmware-2.6.32-504.3.3.el6.noarch.rpm **\Change the kernel\**
3. rpm -ivh https://freed.ga/kernel/kernel-2.6.32-504.3.3.el6.x86_64.rpm --force
4. reboot
5. wget -N --no-check-certificate https://raw.githubusercontent.com/Adair-Hsu/SSR/master/SpeederInstall.sh && bash SpeederInstall.sh **\Install the ServerSpeeder\
```
#### CentOS 7
```
1. wget --no-check-certificate -O rskernel.sh https://raw.githubusercontent.com/hombo125/doubi/master/rskernel.sh && bash rskernel.sh
2. yum install net-tools -y && wget --no-check-certificate -O appex.sh https://raw.githubusercontent.com/0oVicero0/serverSpeeder_Install/master/appex.sh && bash appex.sh install
```

```
1. rpm -ivh http://soft.91yun.pw/ISO/Linux/CentOS/kernel/kernel-3.10.0-229.1.2.el7.x86_64.rpm --force
2. reboot
3. wget -N --no-check-certificate https://github.com/91yun/serverspeeder/raw/master/serverspeeder.sh && bash serverspeeder.sh
```
### Alternate Address for ServerSpeeder Installation
`https://raw.githubusercontent.com/91yun/serverspeeder/master/serverspeeder-all.sh`

### DIY SSR
`vi /etc/shadowsocks.json`
