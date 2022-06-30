# python解析pci config文件

/sys/bus/pci/devices/0000:00:00.0

```
#!/usr/bin/env python3

config_file = open('/sys/bus/pci/devices/0000:00:05.0/config','rb')
n = 0
vendor_id = config_file.read(2)
print("vendor_id:", "0x%s" % vendor_id.hex())
device_id = config_file.read(2)
print("device_id:", "0x%s" % device_id.hex())
command = config_file.read(2)
print("command:", "0x%s" % command.hex())
status = config_file.read(2)
print("status:", "0x%s" % status.hex())
revision = config_file.read(1)
print("revision:", "0x%s" % revision.hex())
class_code = config_file.read(3)
print("class_code:", "0x%s" % class_code.hex())


```

效果：

```
[root@rocky-clion /tmp]# python3 hex.py
vendor_id: 0x8680
device_id: 0x2229
command: 0x0705
status: 0x1000
revision: 0x02
class_code: 0x010601
```



最戳hex解析，没有之一。

























---
