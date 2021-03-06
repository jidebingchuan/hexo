---
title: SNMP
date: 2013-08-01 09:23:28
tags: 协议
---

### 缘起

近期在做公司监控系统，熟悉下常见的协议及支撑范围，其中SNMP（简单网络管理协议）是Internet协议簇的一部分，形成于IETF（互联网工程工作小组）。

### 适用范围

SNMP(simple network management protocol)是因特网架构委员会IAB定义的一个应用层协议。SNMP广泛用于管理和监控网络设备，大多数专业的网络设备都有SNMP agent代理，这些代理被激活和配置后用于和SNMP管理 NMS(network management system)网络管理系统通信。

### 适用场景

典型的用法是配置agent代理，管理机通过agent进行监控和管理。

监控中获取配置的方法是：GET、GETNEXT、GETBULK、TRAP、INFORM。

管理配置和控制的方法是：SET。

管理和配置指令只有网络结构改变的时候才会使用，而监控指令是常态性的工作。

### 基础组件

基于SNMP网络管理系统的基本组件：

1、管理系统。

2、被管理设备的SNMP AGENT。

### SNMP的主要版本

V1,V2均采用明文传送，V3采用加密传送，即SNMPV1,V2用抓包工具能在数据包中直接看到团体名。

v1只使用一种安全策略，团体名(和密码相似)。Agent能够被设置回答哪些团体名(SNMP管理)的查询，很容易让人截取得到团体名或密码。

v2增加了不少额外的安全。首先所有的包信息除了目的地址，其他都被加密(含团体名和源IP地址)。Agent 能够解开加密包获取团体名和源IP地址使请求有效。

v2在安全策略演变时存在多个变种,实际存在多个消息格式。各个v2变种之间的PDU有相同的格式，而总的消息格式又不同。

v3提供三重的安全机制：最高层是认证和私密，中间层提供认证而没有私密，底层没有任何的认证机制和私密。

第一版、第二版（大部分厂商都支持）、第三版（很多厂商不支持）。