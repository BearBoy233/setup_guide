
# 机载计算机

[目录-入门指北](./README.md)


# CUAV C-RTK

CUAV c-rtk-base

CUAV c-rtk 9P

CUAV P9 数传 配置


**硬件参数说明**

 CUAV 官方文档 [http://doc.cuav.net/gps/c-rtk-base/zh-hans/](http://doc.cuav.net/gps/c-rtk-base/zh-hans/)

 [C-RTK-BASE 固件](http://fw.cuav.net/rtk/)

 [奶牛快传/cowtransfer.com](https://cowtransfer.com/s/fc0c30fb355e4c)    **传输口令** `937lf4`

------


[CRTK BASE后台管理 http://192.168.4.1](http://192.168.4.1)

**RTK-Web**  [192.168.4.1](192.168.4.1)

**WIfi Name**	*CUAV_RTK_1B457F*

**WIfi Password**	*cuavrtkbase*


# P900 数传主节点	
  设置为一对多
  *从模块的设备地址 ATS105=[20000,20030)

# 基站一对多设置 [P2M]	[AT&F7	P2M主机]/[AT&F8	P2M从机]

```
操作模式  Master 		#ATS101	[master=0/slave=2]
波特率	  115200 bps	#ATS102	[1-115200/2-57600]
无线速率  230400 bps	#ATS103	[1-230400/3-57600]
无线功率  30dBm (1W)	#ATS108	[30-1000]
通信模式  Point to Multipoint	#ATS133	[0-p2m/1-p2p]
网络ID  23456789	#ATS104	
设备地址  1		#ATS105	[从机=[20000,20030) ]
目标地址  65535		#ATS140	[从机=1]
```

# 基站一对一模式设置 [P2P]	[AT&F10	P2P主机]/[AT&F11	P2P从机]

```
操作模式	Master 
波特率	57600 bps
无线速率	115200 bps
无线功率	30dBm (1W)
通信模式	Point to Point
网络ID	1234567891
设备地址	1
目标地址	2
```
