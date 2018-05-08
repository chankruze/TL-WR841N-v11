# Configuring PPPOE in open-wrt via ssh using uci.sh
```
root@OpenWrt:/lib/config# uci set network.wan.proto=pppoe
root@OpenWrt:/lib/config# uci set network.wan.username='22000621009'
root@OpenWrt:/lib/config# uci set network.wan.password='123456'
root@OpenWrt:/lib/config# uci set network.wan.macaddr='98:de:d0:a2:1c:f1'
root@OpenWrt:/lib/config# uci commit network
root@OpenWrt:/lib/config# ifup wan
root@OpenWrt:/lib/config# 
```
Default `Username` : `root`

Default `Password` : `empty`

Default `IP` : `192.168.133.1`
