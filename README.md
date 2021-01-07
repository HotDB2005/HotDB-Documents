# HotDB-Document

[中文](README.md) | [English](README_en.md)

[中文文档](README.md) | [English Document](README_en.md)

分布式关系型数据库HotDB Server的参考文档。

相关链接：

[官方网站](https://www.hotdb.com)

## 产品介绍

### 概述

**分布式事务数据库 HotDB Server**

HotDB Server是一款实现数据容量和性能横向扩展的交易关系型分布式事务数据库产品。它兼容主流数据库协议和 SQL92/SQL99标准语法，支持自动水平拆分和垂直拆分，能在数据存储分布式化环境下为应用提供集中式数据库的操作体验。为大规模用户、大规模数据、高可用、高并发、高吞吐的业务场景提供强有力的支撑，同时具备强分布式透明、易扩展、易运维、无学习成本等特点。让研发工程师专注应用程序编码实现，无需关心数据的存放位置和操作位置等细节，让数据库工程师更轻松地管理海量数据和海量吞吐的数据库集群，同时提供数据安全、数据容灾、数据恢复、集群监控、智能拓扑、智能大屏、不停机扩容等整套解决方案，适用于TB或PB级的海量数据业务交易场景。

目标：让用户零门槛使用分布式事务数据库和关系型云数据库

### 产品优势

**分布式**

数据分布式集群存储，业务数据支持分库分表，同时提供多种分片算法与表类型，满足用户所需的业务场景。

**强一致**

支持数据强一致性，对全局表、全局序列、分布式事务、副本数据一致、表结构一致、环境配置等都有强一致保障和一致性检测的算法机制。

**智能运维**

可视化参数配置与参数合理性校验，多线程自动化备份，数据态势感知与业务大屏展示，便捷的一键部署整套集群服务，智能数据正确性检测与异常故障及时报警。

**高可用**

计算节点、配置库、底层数据库之间实现三重高可用，不会因为主节点宕机而造成无法提供服务的问题，数据服务的可靠性达到99.999%。

**强透明**

对应用程序全透明，底层在线扩容、备份、OnlineDDL等操作对应用无感知，支持JDBC协议，支持MySQL原生通讯协议，兼容 MySQL 数据库协议及 SQL92 标准语法，覆盖99.9%以上应用开发常用SQL，支持多种数据单库/跨库操作。

**高性能**

计算节点单节点的吞吐量能达到10万+TPS，30万+QPS，并发数可达4096及以上。

### 核心功能

**分库分表**

利用逻辑库方式分库，隔离不同业务属性的数据

可垂直或水平拆分大表，让操作集中于少量数据

内置满足不同业务场景的拆分算法和丰富的表类型

**分布式事务**

支持显示分布式事务与隐式分布式事务

支持弱一致分布式事务与强一致分布式事务

对于应用程序及客户端MySQL命令操作全透明

**跨库操作**

跨库JOIN

跨库UNION

跨库聚合函数

跨库分组排序等

**弹性操作**

通过管理界面实现一键迁库，在线平滑扩容

在线增加只读节点，配置读写分离比重

支持单库向分布式集群的快速迁移

**容灾备份**

保证分布式数据库全局的时间点以及数据状态一致

备份对业务服务无阻塞

支持分布式下的库级别数据备份

支持加密备份文件、计算文件MD5值、备份至远程等功能

**读写分离**

支持数据读写分离功能，且在线设置读写权重

主从延时过大的读节点将自动从读集群中被剔除待恢复正常后再自动加入读集群中

读写分离对上层应用透明，不限制任何SQL语句下发或需要特殊语法处理

**过载保护**

支持对前端连接数总数和用户连接数的限制

控制HotDB发往数据源执行的SQL并发量，保护数据源之间负载平衡，防止某一个数据源因压力过大而宕机

**数据校验**

主备数据一致性检测，支持定时检测与异常检测结果提醒

全局表数据一致性校验

数据路由正确性结果检测

表结构与表索引检测

**在线表结构变更**

管理页面直接进行在线表结构变更操作

执行在线表结构变更期间不阻塞线上业务读写

所有正在执行与执行完成的在线表结构变更记录支持在线查看

### 适用场景

* 高可用
* 高性能
* 海量吞吐
* 海量连接
* 海量并发
* 海量数据
* 海量用户

## 产品文档

[产品白皮书](documents/分布式事务数据库HotDB%20Server产品白皮书-v2.5.6.pdf)

[标准功能使用手册](documents/1.分布式事务数据库HotDB%20Server-v2.5.6【标准】功能使用手册v1.0.pdf)

[管理平台功能使用手册](documents/2.分布式事务数据库HotDB%20Server-v2.5.6【管理平台】功能使用手册v1.0.pdf)

[安装部署功能使用手册](documents/3.分布式事务数据库HotDB%20Server-v2.5.6【安装部署】功能使用手册v1.0.pdf)

[手动升级功能使用手册](documents/4.分布式事务数据库HotDB%20Server-v2.5.6【手动升级】功能使用手册v1.0.pdf)

[服务授权功能使用手册](documents/5.分布式事务数据库HotDB%20Server-v2.5.6【服务授权】功能使用手册v1.0.pdf)

[跨机房灾备功能使用手册](documents/6.分布式事务数据库HotDB%20Server-v2.5.6【跨机房灾备】功能使用手册v1.0.pdf)

[可视化机房切换、修复、移除、演练功能使用手册](documents/7.分布式事务数据库HotDB%20Server-v2.5.6【可视化机房切换、修复、移除、演练】功能使用手册v1.0.pdf)

[管理端命令功能使用手册](documents/8.分布式事务数据库HotDB%20Server-v2.5.6【管理端命令】功能使用手册v1.0.pdf)

[智能巡检功能使用手册](documents/9.分布式事务数据库HotDB%20Server-v2.5.6【智能巡检】功能使用手册v1.0.pdf)

[名词解释功能使用手册](documents/10.分布式事务数据库HotDB%20Server-v2.5.6【名词解释】功能使用手册v1.0.pdf)

[参数说明列表](documents/12.HotDB%20Server&管理平台参数说明列表_2.5.6.xlsx)

[集群环境要求说明](documents/13.分布式事务数据库HotDB%20Server-【集群环境要求说明】V1.0.xlsx)

[计算节点错误码](documents/14.分布式事务数据库HotDB%20Server-v2.5.6【计算节点错误码】v1.0.xlsx)

[硬件配置推荐](documents/15.分布式事务数据库产品HotDB%20Server硬件配置推荐---热璞科技v3.2.xlsx)

## 往期文章

[［原创］热璞数据库HotDB开放下载先知——安装部署篇三（自动部署）](https://blog.csdn.net/m0_46473154/article/details/111317799)

[［原创］热璞数据库HotDB开放下载先知————安装部署（二）](https://blog.csdn.net/m0_46473154/article/details/111312511)

[［原创］HotDB开放下载先知————安装部署第一篇](https://blog.csdn.net/m0_46473154/article/details/111310295)

[［原创］【管理平台新增功能】热璞数据库HotDB 2.5.6来了，新功能get起来第一篇](https://blog.csdn.net/m0_46473154/article/details/111225615)

[［原创］识别国产分布式事务数据库核心算法之—四大功能谎言](https://blog.csdn.net/m0_46473154/article/details/110425399)

[［原创］国产分布式事务数据库在金融领域的实战经验](https://blog.csdn.net/m0_46473154/article/details/110424974)

[［原创］【新功能解读一】HotDB Server V2.5.6支持计算节点服务数量在线水平扩容](https://blog.csdn.net/m0_46473154/article/details/109854585)

[［原创］标杆快线——热璞数据库助力城轨数字化建设，促进城市经济腾飞](https://blog.csdn.net/m0_46473154/article/details/109490601)

[［原创］分布式事务数据跨机房灾备](https://blog.csdn.net/m0_46473154/article/details/109102238)

[［原创］分布式事务数据库HotDB——解决集中式数据库面临的挑战](https://blog.csdn.net/m0_46473154/article/details/109074454)

[［原创］热璞数据库HotDB跨JOIN功能介绍](https://blog.csdn.net/m0_46473154/article/details/108261460)

[［原创］热璞数据库HotDB读写分离介绍](https://blog.csdn.net/m0_46473154/article/details/108261353)

[［原创］HotDB分片方案在线变更(特色功能之一）](https://blog.csdn.net/m0_46473154/article/details/107984693)

[［原创］HotDB一键迁库介绍](https://blog.csdn.net/m0_46473154/article/details/107980832)

[［原创］热璞数据库HotDB Backup介绍](https://blog.csdn.net/m0_46473154/article/details/107979941)

[［原创］纯干货预警--聊一聊MySQL 数据库内存管理](https://blog.csdn.net/m0_46473154/article/details/107659796)

[［原创］热璞数据库HotDB智能大屏](https://blog.csdn.net/m0_46473154/article/details/107542615)

[［原创］热璞数据库HotDB数据分片预测](https://blog.csdn.net/m0_46473154/article/details/107541167)

[［原创］热璞数据库HotDB分片方案智能推荐](https://blog.csdn.net/m0_46473154/article/details/107540693)

[［原创］热璞数据库HotDB水平分片表的分片规则](https://blog.csdn.net/m0_46473154/article/details/107519576)

[［原创］热璞数据库Hot DB数据容量如何？](https://blog.csdn.net/m0_46473154/article/details/107518804)

[［转载］实力验证—— 热璞数据库以卓越的产品性能成为首批通过信通院金融数据库性能测评厂商](https://blog.csdn.net/m0_46473154/article/details/107343613)

[［原创］国产化联合——热璞数据库携手天玑数据推出分布式事务数据库一体机联合解决方案](https://blog.csdn.net/m0_46473154/article/details/107184109)

[［原创］热璞数据库HotDB干货分享来啦——深度解析innodb_rollback_on_timeout的作用](https://blog.csdn.net/m0_46473154/article/details/107067304)

[［原创］热璞数据HotDB库简介](https://blog.csdn.net/m0_46473154/article/details/106789705)

[［原创］HotDB Server运行相关——计算节点启动说明](https://blog.csdn.net/m0_46473154/article/details/106361795)

[［原创］热璞数据库教你实力避坑 ，MySQL数据高可用进阶版详解出炉](https://blog.csdn.net/m0_46473154/article/details/106232070)

[［原创］分享——热璞数据库HotDB助力南京市民卡数字化转型案例](https://blog.csdn.net/m0_46473154/article/details/106123385)

[［转载］国产数据库清单（2020年第1季度）](https://blog.csdn.net/m0_46473154/article/details/105977550)

[［原创］热璞数据库HotDB行业中应用的客户案例](https://blog.csdn.net/m0_46473154/article/details/105953961)

[［原创］详解热璞数据库如HotDB如何真正实现数据高可用](https://blog.csdn.net/m0_46473154/article/details/105820442)

[［原创］热璞数据库HotDB Server 提供7种数据拆分算法，满足用户大部分场景的需求](https://blog.csdn.net/m0_46473154/article/details/105787051)

[［原创］分布式数据库下的死锁检测](https://blog.csdn.net/m0_46473154/article/details/105786214)

[［原创］不同业务场景该如何选择数据库类型？每种类型有哪些代表性的产品？](https://blog.csdn.net/m0_46473154/article/details/105774272)

[［原创］分布式事务数据库HotDB：数据节点增加的弹性扩容线性系数测试验证](https://blog.csdn.net/m0_46473154/article/details/105771695)

[［原创］应用层和分布式事务数据库两种数据分片方式的核心区别](https://blog.csdn.net/m0_46473154/article/details/105654936)

[［原创］分布式事务数据库HotDB硬件配置](https://blog.csdn.net/m0_46473154/article/details/105653839)

[［原创］分布式事务数据库安全技术指南](https://blog.csdn.net/m0_46473154/article/details/105534030)

[［原创］金融行业国产OLTP分布式数据库如何选型](https://blog.csdn.net/m0_46473154/article/details/105529158)

[［原创］热璞数据库HotDB Server 安装部署手册](https://blog.csdn.net/m0_46473154/article/details/105428667)

[［原创］分布式事务数据库HotDBV2.5.4版本](https://blog.csdn.net/m0_46473154/article/details/105247281)

[［原创］探讨 急需突破传统模式实现数字化转型的金融行业，该如何拥自己的分布式事务数据—自研？购买？](https://blog.csdn.net/m0_46473154/article/details/105220251)

[［原创］分布式事务数据库HotDBV2.5.3版本](https://blog.csdn.net/m0_46473154/article/details/105137948)

[［原创］分布式事务数据库HotDBV2.5.3版本](https://blog.csdn.net/m0_46473154/article/details/105137948)

[［原创］MySQL数据库架构选型](https://blog.csdn.net/m0_46473154/article/details/105119279)

[［原创］分布式事务数据库产品V2.5.2版本](https://blog.csdn.net/m0_46473154/article/details/105084908)

[［原创］洋山深水港四期建设中分布式事务数据库HotDB的关键作用](https://blog.csdn.net/m0_46473154/article/details/105083635)

[［原创］官方提供分布式事务数据库HotDB免费试用路径](https://blog.csdn.net/m0_46473154/article/details/105047792)

[［原创］浅谈 如何选择适配数据库](https://blog.csdn.net/m0_46473154/article/details/105047428)

[［原创］分布式事务数据库HotDBv2.5.1版本](https://blog.csdn.net/m0_46473154/article/details/105018602)

[［原创］分布式事务数据库产品HotDBV2.5.0版本](https://blog.csdn.net/m0_46473154/article/details/104979546)

[［原创］分布式事务数据库HotDB产品的优势](https://blog.csdn.net/m0_46473154/article/details/104754880)

[［原创］数据库环境类别](https://blog.csdn.net/m0_46473154/article/details/104675235)

[［原创］分布式事务数据库的数据分片规则](https://blog.csdn.net/m0_46473154/article/details/104674204)

[［原创］MySQL数据库的服务器配置选型建议以及部署规划](https://blog.csdn.net/m0_46473154/article/details/104670881)
