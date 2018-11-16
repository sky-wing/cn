# 计费概述
## 实例收费标准
分布式关系型数据库 DRDS 实例的收费标准依据实例的规格进行收费，即实例的CPU核数和内存大小。 DRDS本身不存储数据，所以规格与磁盘大小无关

## 实例到期/欠费说明
以下是 DRDS 实例欠费或者到期的保留政策。

|计费类型|实例到期/欠费处理逻辑|
|---|---|
|包年包月|实例到期后，会被标记为到期状态，数据库服务不可用，如 7 天内未续费，则 7 天后会被删除，同时实例对应的备份文件也会被删除，实例数据不能恢复。|
|按配置|实例欠费后，会被标记为欠费状态，数据库服务不可用，如 7 天后仍欠费，则会被删除，同时实例对应的备份文件也会被删除，实例数据不能恢复。|

DRDS 实例在到期或欠费后会有消息提醒，请注意查收，及时续费，以免数据被删除无法找回。
计费与通知相关信息，详情请查看：<br>
- [预付费计费说明](../../../Finance/Billing/Billing-method/Prepay.md) 
- [后付费计费说明](../../../Finance/Billing/Billing-method/Postpay.md) 