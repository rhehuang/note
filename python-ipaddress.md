```python
# -*- coding:utf-8 -*-
import ipaddress

# 网络号
str_network_address=ipaddress.ip_network("192.168.1.0/24",strict=False).network_address

# 广播地址
str_broadcast_address=ipaddress.ip_network("192.168.1.0/24",strict=False).broadcast_address

# 可用IP地址
ipList=list(ipaddress.ip_network("192.168.1.0/24",strict=False).hosts())

print('网络号',str_network_address)
print('广播地址',str_broadcast_address)
print(ipList)
```
