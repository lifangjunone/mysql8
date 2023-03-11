## mysql base

常用命令

```shell
1. 查看最大链接数
select @@max_connections
2. 查看 连接数（有多少人正在连接）, 也就是连接线程数
show processlist 
show full processlist
```

Mysql Server 层：
一. mysql 连接管理【 Connection Management】
   1. mysql链接客户端
   2. 连接管理模块
      1. 建立tcp链接
      2. 用户密码验证
      3. 连接数判断
二. 管理服务和一些工具 【 Management service & Utilties】
   1. 配置
   2. 数据库备份，迁移
   3. 安全
   4. 元数据
   5. 插件
三. SQL Interface
   1. DDL
   2. DML
   3. function
   4. view
   5. triggers
   6. procedures
   7. JSON
四. Parser【解析器】
五. Optimizer 【优化器】
   1. explain
六. Cache & Buffers 【缓存、缓冲】
