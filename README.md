﻿12306
=====

我要回家过年

### 新人上手
https://github.com/12306NgPM/12306ngpm/wiki/%E6%96%B0%E4%BA%BA%E4%B8%8A%E6%89%8B

### 使用说明
1. 下载并安装Virtual Box 4.2: https://www.virtualbox.org/wiki/Downloads
2. 下载并安装Vagrant: http://vagrantup.com/
3. 第一次运行时,打开命令行，进入源代码的根目录,执行（如果是windows平台，在下面的命令后面加.bat后缀）：
   
   vagrant box add base http://files.vagrantup.com/lucid32.box

   vagrant up
   
4. 下次就只需要执行下面的命令就可以使用:
   
   vagrant up

5. 如果是windows平台，用putty登录：127.0.0.1:2222，用户名/密码：vagrant/vagrant
6. 如果是非Windows平台
   
   vagrant ssh server
   vagrant ssh client
   
7. 进入工作主目录 - 这个虚拟机上的主目录是你宿主机执行vagrant命令的目录
   
   cd /vagrant/trunk/tpms

   mvn compile exec:java
   
8. 顺利的话,你应该可以看到BUILD SUCCESS的字样,如有任何问题,欢迎到下面的链接上报BUG:
   http://bugzilla.12306ng.org/
   
9. 如果需要执行测试用例的话,请执行
   
   cd /vagrant/trunk/tpms

   mvn test
