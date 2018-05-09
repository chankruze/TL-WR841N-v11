# Back To Original Firmware
## Case I
If you have a web gui based open-wrt firmware then simply select the firmware file & update firmware via webinterface (luci).

## Case II
If you flashed a open-wrt which doesn't have a webinterface or due to misconfiguration if you are unable to open the webinterface which is http://192.168.1.1 then follow this method.

1. Upload the firmware renamed to short name like firmware.bin to a http upload service (http://www.fast-files.com/).
2. Reset the router configuration by holding reset hardware buttown
3. Then ssh to 192.168.1.1 & follow bellow snippet.
```
cd /tmp
wget http://www.example.org/original_firmware.bin
mtd -r write /tmp/original_firmware.bin firmware
```
For example for my case i used these code :
compare it:
![My Snippet](https://image.ibb.co/k8DCM7/Screenshot_from_2018_05_09_09_29_27.png)

My Firmware is hosted on : http://www.321webs.com/sendfile/161439ad.htm
