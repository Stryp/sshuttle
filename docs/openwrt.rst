OpenWRT
========

Run::

    opkg install python3 python3-pip iptables-mod-extra iptables-mod-nat-extra iptables-mod-ipopt
    python3 /usr/bin/pip3 install sshuttle
    sshuttle -l 0.0.0.0 -r <IP> -x 192.168.1.1 0/0

Please note::

- iptables-mod* packages must be installed in the same drive where iptables itself is running. 
- If you want to use the --daemon flag you have to replace dropbear with openssh-client:
https://oldwiki.archive.openwrt.org/inbox/replacingdropbearbyopensshserver
