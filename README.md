# linux-
#网卡解决network和NetworkManager的冲突问题
方法1：
[root@bigpeng ~]# systemctl disable NetworkManager
Removed symlink /etc/systemd/system/multi-user.target.wants/NetworkManager.service.
Removed symlink /etc/systemd/system/dbus-org.freedesktop.NetworkManager.service.
Removed symlink /etc/systemd/system/dbus-org.freedesktop.nm-dispatcher.service.
[root@bigpeng ~]# systemctl stop NetworkManager.service 

方法2：
systemctl restart NetworkManager
