# “树”的奥秘
---
Linux就是一棵树，它没有Windows的C盘D盘什么的，所有的文件和设备都以文件的形式挂接在树枝上。


## 3.1 Linux的文件组织结构
在Linux操作系统下，绝大多数软件都是被安装在既定位置的，形成了一种规范行为。

## 3.2 基本组织原则

## 3.3 根文件系统

### 3.3.1 原则与特性
保证根分区的精巧：  
  1.根文件系统包含了很多系统特有的配置文件，如：内核、hostname等。这些都是系统特有的，也就意味着不能通过网络系统共享。  
  2.开发者不能将根分区开发得太大，导致有人使用了更小的根分区而无法安装。  
  3.磁盘分区越大，发生故障的概率也就越高。  
### 3.3.2 必备的内容
  bin boot dev etc lib media mnt opt sbin srv tmp usr var
  
### 3.3.3 可选的内容
  home lib64 root
  
## 3.4 子目录
### 3.4.1 /bin目录——Shell命令
  1.必备内容
  cat chgrp chmod chown cp date dd df dmesg echo false hostname kill ln login ls mkdir mknod more mount mv ps pwd rm rmdir sed sh stty su true umount uname
  2.可选内容
  csh ed tar cpio gzip gunzip zcat netstat ping
  
### 3.4.2 /boot目录——启动过程所需内容
  推荐单独分区
  
### 3.4.3 /dev目录——设置文件
### 3.4.4 /etc目录——配置文件
  “只读”是指在系统的运行期间内极少变动的。
  1.需要放在/etc下的子目录
  opt rc.d X11 sgml xml
  2.需要放在/etc下的文件
  csh.login exports fstab ftpusers gateways group host.conf hosts hosts.allow hosts.deny hosts.equiv hosts.lpd inetd.conf inittab issue ld.so.conf motd mtab mtools.conf networks passwd printcap profile protocols reslov.conf rpc securetty services shells syslog.conf
  
