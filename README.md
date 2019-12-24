# OpenVPN Install for Multiple Users
Share the same client-certificate with everyone. This script pre-enabled the duplicate-cn.
[![HitCount](http://hits.dwyl.io/gayanvoice/openvpn-install-for-multiple-users.svg)](http://hits.dwyl.io/gayanvoice/openvpn-install-for-multiple-users)

## Watch video
[![Install OpenVPN for multiple users on Ubuntu](https://img.youtube.com/vi/lBelfmMkQYU/0.jpg)](https://www.youtube.com/watch?v=lBelfmMkQYU)

## Installation
Run this script
```
wget https://git.io/JeFPU -O openvpn-install.sh && bash openvpn-install.sh
```
## OpenVPN Server
* Start
```
service openvpn start
```
* Status
```
service openvpn status
```
* Stop
```
service openvpn stop
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

## Prerequisites
* Ubuntu 16.04 is no longer supported, use a latest version of OS
* Only works with Debian, Ubuntu or CentOS
* Enable 'tun' device before running this script
```
cat /dev/net/tun
# if you receive this message, your 'tun' device is running
# cat: /dev/net/tun: File descriptor in bad state
```
* This script run on 'bash', not 'sh' for Debian users
```
echo {$BASH_VERSION}
```
* Run this as 'root'
```
sudo su
```
