# pciutils-3.7.0 学习



```
Something I hope you know before go into the coding~
First, please watch or star this repo, I'll be more happy if you follow me.
Bug report, questions and discussion are welcome, you can post an issue or pull a request.
```

## 软件信息

```
[root@rocky ~]# yum info pciutils
Last metadata expiration check: 0:19:02 ago on Wed 29 Jun 2022 09:29:49 PM CST.
Installed Packages
Name         : pciutils
Version      : 3.7.0
Release      : 1.el8
Architecture : x86_64
Size         : 211 k
Source       : pciutils-3.7.0-1.el8.src.rpm
Repository   : @System
From repo    : anaconda
Summary      : PCI bus related utilities
URL          : http://atrey.karlin.mff.cuni.cz/~mj/pciutils.shtml
License      : GPLv2+
Description  : The pciutils package contains various utilities for inspecting and
             : setting devices connected to the PCI bus.

[root@rocky ~]# rpm -ql pciutils
/lib64/libpci.so.3
/lib64/libpci.so.3.6.4

/sbin/lspci
/sbin/setpci
/sbin/update-pciids

/usr/share/doc/pciutils/COPYING
/usr/share/doc/pciutils/ChangeLog
/usr/share/doc/pciutils/README
/usr/share/doc/pciutils/pciutils.lsm
```


## 目录



















---
