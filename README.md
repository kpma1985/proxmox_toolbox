# proxmox_toolbox

## Tonton Jo - 2021
Join me on Youtube: https://www.youtube.com/c/tontonjo

If you find this usefull, please think about [Buying me a coffee](https://www.buymeacoffee.com/tontonjo)
and to [Subscribe to my youtube channel](http://youtube.com/channel/UCnED3K6K5FDUp-x_8rwpsZw?sub_confirmation=1)

This little tool aim to get smalls one-time configurations for Proxmox Virtual environement and backup server hosts in no time.

![screenshot](https://i.ibb.co/xYfyt3f/Screenshot-2021-06-04-095759.png)  
## Features are:
- Install usefull dependencies: ifupdown2, git, sudo
- Hide enterprise repo and set no-subscription repository
- Configure email service to send system and proxmox notifications (postfix)
- Enhance security a bit with the following:
- - Enable fail 2 ban with default configuration for sshd, proxmox virtual environement and backup server (credits to [inettgmbh](https://github.com/inettgmbh/fail2ban-proxmox-backup-server))
- - Create another user with sudo rights
- - Disable root ssh login
- - Create another Proxmox administrator and disabling Root user
- Update host, and when no-enterprise source is set - disable no-subscription message
- Enable SNMP V2 or v3 - you choose - with a default working configuration

## USAGE
You can use this tool either with:
```shell
git clone https://github.com/Tontonjo/proxmox_toolbox.git
```
```shell
bash proxmox_toolbox/proxmox_toolbox.sh
```
OR
```shell
wget https://raw.githubusercontent.com/Tontonjo/proxmox_toolbox/main/proxmox_toolbox.sh
```
```shell
bash proxmox_toolbox.sh
```

## SOURCES:
https://pve.proxmox.com/wiki/Fail2ban  
https://github.com/inettgmbh/fail2ban-proxmox-backup-server  
https://forum.proxmox.com/threads/how-do-i-set-the-mail-server-to-be-used-in-proxmox.23669/  
https://linuxscriptshub.com/configure-smtp-with-gmail-using-postfix/  
https://suoption_pickedpport.google.com/accounts/answer/6010255  
https://www.howtoforge.com/community/threads/solved-problem-with-outgoing-mail-from-server.53920/  
http://mhawthorne.net/posts/2011-postfix-configuring-gmail-as-relay/  
https://docs.oracle.com/en/cloud/cloud-at-customer/occ-get-started/add-ssh-enabled-user.html  
https://www.noobunbox.net/serveur/monitoring/configurer-snmp-v3-sous-debian  
https://github.com/DeadlockState/Proxmox-prepare  
