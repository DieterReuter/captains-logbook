# HowTo: re-install VMware Fusion

I you have any weired problems with networking it's sometimes better to re-install
VMware Fusion from scratch. But as a first step, clean the app and all settings from
the disk.


- remove VMware Fusion
```
sudo rm -fr /Applications/VMware Fusion.app
```

- remove all VMware Fusion settings
```
sudo rm -fr /Library/Preferences/VMware\ Fusion
sudo rm -fr /var/db/vmware/
```


## Re-install VMware Fusion 8.1.1
- import your license

After installing, just check the VMware networking. `vmnet1` and `vmnet8` should be present.
```
ifconfig | grep vmnet
...
vmnet1: flags=8863<UP,BROADCAST,SMART,RUNNING,SIMPLEX,MULTICAST> mtu 1500
	ether 00:50:56:c0:00:01
	inet 172.16.184.1 netmask 0xffffff00 broadcast 172.16.184.255
vmnet8: flags=8863<UP,BROADCAST,SMART,RUNNING,SIMPLEX,MULTICAST> mtu 1500
	ether 00:50:56:c0:00:08
	inet 192.168.90.1 netmask 0xffffff00 broadcast 192.168.90.255
```

Check if the ``*.leases` files are in place.
```
ls -al /var/db/vmware/
total 16
drwxr-xr-x   6 root  wheel   204 Aug  6 16:57 .
drwxr-xr-x  77 root  wheel  2618 Aug  6 16:57 ..
-rw-r--r--   1 root  wheel   417 Aug  6 16:57 vmnet-dhcpd-vmnet1.leases
-rw-r--r--   1 root  wheel     0 Aug  6 16:57 vmnet-dhcpd-vmnet1.leases~
-rw-r--r--   1 root  wheel   417 Aug  6 16:57 vmnet-dhcpd-vmnet8.leases
-rw-r--r--   1 root  wheel     0 Aug  6 16:57 vmnet-dhcpd-vmnet8.leases~
```

List all the VMware Fusion settings files.
```
ls -al /Library/Preferences/VMware\ Fusion
total 24
drwxr-xr-x   8 root  wheel   272 Aug  6 16:57 .
drwxr-xr-x  53 root  wheel  1802 Aug  6 16:12 ..
-r--r--r--   1 root  wheel    31 Aug  6 16:57 lastLocationUsed
-rw-r--r--   1 root  wheel   543 Jul 24 18:53 license-fusion-80-e1-201505
-rw-r--r--   1 root  wheel   462 Apr 15 02:59 networking
drwxr-xr-x@ 10 root  wheel   340 Aug  6 16:57 thnuclnt
drwxr-xr-x   3 root  wheel   102 Aug  6 16:57 vmnet1
drwxr-xr-x   5 root  wheel   170 Aug  6 16:57 vmnet8
```


## Manually Add and Remove VMware Fusion Virtual Adapters
see the followiing tutorial https://thornelabs.net/2013/10/18/manually-add-and-remove-vmware-fusion-virtual-adapters.html
