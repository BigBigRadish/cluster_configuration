这里注意啊,单机情况下,
我们使用两个ip
其中主机是ubuntu
从机是localhost
需要在/etc/hosts中做好映射,例如:
10.85.13.74 ubuntu
127.0.0.1 localhost

另外,如果使用wlan0或者有线网中DHCP,IP地址不固定的话,每次启动
HDFS前都需要在/etc/hosts把hostname的映射ip改为ifconfig中wlan0或者有线网的ip.
否则HDFS启动会报错.
