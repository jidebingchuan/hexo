---
title: NET-SNMP
date: 2013-08-01 11:36:58
tags: 协议
---

### 缘起

采集的MIB库信息有了之后，那么就是选择拉的方式还是推的方式采集数据，拉的方式由监控系统轮询各个系统的代理获取系统指标数据，例如温度、风扇转速、IO、内存等指标数据；推的方式由SNMP的代理端主动推送一条数据给数据管理端（SNMP Trap）。

### NET-SNMP

在 Linux 系统中，我们可以选择 net-snmp 来处理绝大多数和 SNMP 相关的工作。

NET-SNMP 是一种开放源代码的 SNMP 协议实现。它支持 SNMP v1, SNMP v2c 与 SNMP v3，并可以使用 IPV4 及 IPV6 。也包含 SNMP Trap 的所有相关实现。Net-snmp 包含了 snmp 实用程序集和完整的 snmp 开发库。

用户使用 net-snmp 提供的工具，可以完成很多关于 SNMP 的操作。

### 功能特性

命令行应用程序

1. 支持SNMP的设备获得数据.支持独立请求 (snmpget, snmpgetnext), 与重复请求 (snmpwalk, snmptable, snmpdelta).
2. 支持SNMP的设备配置属性.(snmpset).
3. 支持SNMP的设备获取特定的信息.(snmpdf, snmpnetstat, snmpstatus).
4. 将MIB OIDs的两种表现形式(数字及文字)相互转换.并显示MIB的内容与结构(snmptranslate).

### 基础组件

- 一个图形化的MIB浏览器(tkmib，基于Tk/perl).
- 一个接收SNMP提示消息(SNMP traps)的守护程序.(snmptrapd).可以将选定的SNMP消息记录到系统日志(syslog),NT 事件日志(NT Event Log),文本文件中.或是转发到其它的SNMP管理程序,也可以传给外部的应用程序.
- 一个回应SNMP查询的客户端.(snmpd).它集成了大量SNMP的模块.并可通过动态链接库,外部脚本与命令,多路SNMP技术(SMUX),以及可扩客户端协议(AgentX)进行扩展.
- 一个用来开发SNMP应用程序的程序库.支持 C 与 perl 的 APIs.防对方是否