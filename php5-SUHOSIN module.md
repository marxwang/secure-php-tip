

#介紹 (from 官網)

About | SUHOSIN
https://suhosin.org/stories/index.html

Suhosin (pronounced 'su-ho-shin') is an advanced protection system for PHP installations. It was designed to protect servers and users from known and unknown flaws in PHP applications and the PHP core.


#安裝指引

##ref
Debian 8 and Ubuntu 14.04 LTS Install Suhosin PHP Extension To Protect Your Server
http://www.cyberciti.biz/faq/debian-8-ubuntu-14-04-lts-install-suhosin-extension-command/


##安裝步驟 (ubuntu/debian)

###1. 添加 repo /etc/apt/sources.list

ubuntu trusty
```
sudo -s
echo 'deb http://repo.suhosin.org/ ubuntu-trusty main' >> /etc/apt/sources.list
apt-get update
```

Debian Linux 8.x   
```
sudo -s
echo 'deb http://repo.suhosin.org/ debian-jessie main' >> /etc/apt/sources.list
apt-get update
```

###2. 加 apt-key
```
//add key
wget https://sektioneins.de/files/repository.asc 
sudo apt-key add repository.asc
```
###3. 安裝php5-suhosin-extension  
```
sudo apt-get update
sudo apt-get install php5-suhosin-extension
```
