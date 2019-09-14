# OpenVPN Install for Multiple Users
Share the same client-certificate with everyone | Enabled duplicate-cn | Best for VPN startups
## Prerequisites
* Ubuntu 16.04 is no longer supported, use a latest version of OS
* Enable 'tun' device before running this script
* Only works with Debian, Ubuntu or CentOS
* This script run on 'bash', not 'sh' for Debian users
* Run this as 'root'
```
sudo su
```

## Installation
Run this script
```
wget https://git.io/JeYgM -O openvpn-install.sh && bash openvpn-install.sh
```

## Remove
* Uninstall OpenVPN
```
sudo apt remove openvpn
```

* Remove it's dependencies
```
sudo rm -rfv /etc/openvpn
```
