---
title: SNMP采集华三设备温度
date: 2013-08-19 12:24:10
tags: 监控
---

单板上各个传感器的温度信息：hh3cEntityExtTemperature

节点OID值：1.3.6.1.4.1.25506.2.6.1.1.1.1.12

获取单板上各个传感器的温度信息：

可以参考MIB节点实体描述信息entPhysicalDescr，节点的OID值：1.3.6.1.2.1.47.1.1.1.1.2，实体名称信息entPhysicalName，节点的OID值：1.3.6.1.2.1.47.1.1.1.1.7。

温度的详细信息可以参考命令行display environment。

174: hh3cEntityExtTemperature.17663 (integer) 31

175: hh3cEntityExtTemperature.17664 (integer) 36

176: hh3cEntityExtTemperature.17665 (integer) 37

177: hh3cEntityExtTemperature.17679 (integer) 32

178: hh3cEntityExtTemperature.17680 (integer) 36

179: hh3cEntityExtTemperature.17681 (integer) 37

180: hh3cEntityExtTemperature.17695 (integer) 34

181: hh3cEntityExtTemperature.17696 (integer) 38

182: hh3cEntityExtTemperature.17697 (integer) 36

183: hh3cEntityExtTemperature.17743 (integer) 32

184: hh3cEntityExtTemperature.17744 (integer) 50

185: hh3cEntityExtTemperature.17745 (integer) 42



174: entPhysicalDescr.17663 (octet string) Temperature Sensor on Board [54.65.6D.70.65.72.61.74.75.72.65.20.53.65.6E.73.6F.72.20.6F.6E.20.42.6F.61.72.64 (hex)]

175: entPhysicalDescr.17664 (octet string) Temperature Sensor on Board [54.65.6D.70.65.72.61.74.75.72.65.20.53.65.6E.73.6F.72.20.6F.6E.20.42.6F.61.72.64 (hex)]

176: entPhysicalDescr.17665 (octet string) Temperature Sensor on Board [54.65.6D.70.65.72.61.74.75.72.65.20.53.65.6E.73.6F.72.20.6F.6E.20.42.6F.61.72.64 (hex)]

177: entPhysicalDescr.17679 (octet string) Temperature Sensor on Board [54.65.6D.70.65.72.61.74.75.72.65.20.53.65.6E.73.6F.72.20.6F.6E.20.42.6F.61.72.64 (hex)]

178: entPhysicalDescr.17680 (octet string) Temperature Sensor on Board [54.65.6D.70.65.72.61.74.75.72.65.20.53.65.6E.73.6F.72.20.6F.6E.20.42.6F.61.72.64 (hex)]

179: entPhysicalDescr.17681 (octet string) Temperature Sensor on Board [54.65.6D.70.65.72.61.74.75.72.65.20.53.65.6E.73.6F.72.20.6F.6E.20.42.6F.61.72.64 (hex)]

180: entPhysicalDescr.17695 (octet string) Temperature Sensor on Board [54.65.6D.70.65.72.61.74.75.72.65.20.53.65.6E.73.6F.72.20.6F.6E.20.42.6F.61.72.64 (hex)]

181: entPhysicalDescr.17696 (octet string) Temperature Sensor on Board [54.65.6D.70.65.72.61.74.75.72.65.20.53.65.6E.73.6F.72.20.6F.6E.20.42.6F.61.72.64 (hex)]

182: entPhysicalDescr.17697 (octet string) Temperature Sensor on Board [54.65.6D.70.65.72.61.74.75.72.65.20.53.65.6E.73.6F.72.20.6F.6E.20.42.6F.61.72.64 (hex)]

183: entPhysicalDescr.17743 (octet string) Temperature Sensor on Board [54.65.6D.70.65.72.61.74.75.72.65.20.53.65.6E.73.6F.72.20.6F.6E.20.42.6F.61.72.64 (hex)]

184: entPhysicalDescr.17744 (octet string) Temperature Sensor on Board [54.65.6D.70.65.72.61.74.75.72.65.20.53.65.6E.73.6F.72.20.6F.6E.20.42.6F.61.72.64 (hex)]

185: entPhysicalDescr.17745 (octet string) Temperature Sensor on Board [54.65.6D.70.65.72.61.74.75.72.65.20.53.65.6E.73.6F.72.20.6F.6E.20.42.6F.61.72.64 (hex)]



174: entPhysicalName.17663 (octet string) inflow Sensor 1/0/1 [69.6E.66.6C.6F.77.20.53.65.6E.73.6F.72.20.31.2F.30.2F.31 (hex)]

175: entPhysicalName.17664 (octet string) outflow Sensor 1/0/1 [6F.75.74.66.6C.6F.77.20.53.65.6E.73.6F.72.20.31.2F.30.2F.31 (hex)]

176: entPhysicalName.17665 (octet string) hotspot Sensor 1/0/1 [68.6F.74.73.70.6F.74.20.53.65.6E.73.6F.72.20.31.2F.30.2F.31 (hex)]

177: entPhysicalName.17679 (octet string) inflow Sensor 1/1/1 [69.6E.66.6C.6F.77.20.53.65.6E.73.6F.72.20.31.2F.31.2F.31 (hex)]

178: entPhysicalName.17680 (octet string) outflow Sensor 1/1/1 [6F.75.74.66.6C.6F.77.20.53.65.6E.73.6F.72.20.31.2F.31.2F.31 (hex)]

179: entPhysicalName.17681 (octet string) hotspot Sensor 1/1/1 [68.6F.74.73.70.6F.74.20.53.65.6E.73.6F.72.20.31.2F.31.2F.31 (hex)]

180: entPhysicalName.17695 (octet string) inflow Sensor 1/2/1 [69.6E.66.6C.6F.77.20.53.65.6E.73.6F.72.20.31.2F.32.2F.31 (hex)]

181: entPhysicalName.17696 (octet string) outflow Sensor 1/2/1 [6F.75.74.66.6C.6F.77.20.53.65.6E.73.6F.72.20.31.2F.32.2F.31 (hex)]

182: entPhysicalName.17697 (octet string) hotspot Sensor 1/2/1 [68.6F.74.73.70.6F.74.20.53.65.6E.73.6F.72.20.31.2F.32.2F.31 (hex)]

183: entPhysicalName.17743 (octet string) inflow Sensor 1/5/1 [69.6E.66.6C.6F.77.20.53.65.6E.73.6F.72.20.31.2F.35.2F.31 (hex)]

184: entPhysicalName.17744 (octet string) outflow Sensor 1/5/1 [6F.75.74.66.6C.6F.77.20.53.65.6E.73.6F.72.20.31.2F.35.2F.31 (hex)]

185: entPhysicalName.17745 (octet string) hotspot Sensor 1/5/1 [68.6F.74.73.70.6F.74.20.53.65.6E.73.6F.72.20.31.2F.35.2F.31 (hex)]



通过174: hh3cEntityExtTemperature.17663 (integer) 31

174: entPhysicalDescr.17663 (octet string) Temperature Sensor on Board [54.65.6D.70.65.72.61.74.75.72.65.20.53.65.6E.73.6F.72.20.6F.6E.20.42.6F.61.72.64 (hex)]

174: entPhysicalName.17663 (octet string) inflow Sensor 1/0/1 [69.6E.66.6C.6F.77.20.53.65.6E.73.6F.72.20.31.2F.30.2F.31 (hex)]

可以看出1号框0号槽位，inflow Sensor 1的温度31度。