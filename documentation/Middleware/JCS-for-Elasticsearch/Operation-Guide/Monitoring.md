## 监控集群
单击集群名称进入集群详情页，可以查看关于集群运行的详细监控信息，辅助集群运维监管。也可由“云监控-资源监控-云搜索Elasticsearch”监控进入查看。</br>
1. 单击刷新图标可刷新页面内状态，图片支持放大功能。</br>
2. 时长选择项：监控时段可选择据当前时间“15分钟”、“1小时”、“6小时”、“1天”、“7天”、“30天”，也可由日历时间段自主选择。</br>
3. 单击右上方“设置报警规则”，单击跳转至云监控页面进行报警规则的设置。</br>
![查询1](https://github.com/jdcloudcom/cn/blob/Elasticsearch/image/Internet-Middleware/JCS%20for%20Elasticsearch/监控集群-01.png)
 
监控指标包括：集群健康状态、集群查询QPS、集群写入QPS、节点CPU使用率、节点磁盘使用率、节点HeapMemory使用率。</br>

| 监控项	| 说明	|
|:--:|:--:|
| 集群状态 | 0 表示绿色，此时集群处于最健康状态；1 表示黄色，此时集群的高可用性受到影响，但是搜索结果仍然完整；2 表示红色，此时集群异常，搜索只能返回部分数据 |
| 集群查询QPS（Count/Second） 	| 反应集群查询操作繁忙程度 |
| 集群写入QPS（Count/Second） | 反应集群写入操作繁忙程度 |
| CPU节点利用率（%） | CPU 使用率过高会导致集群节点处理能力下降，甚至宕机 |
| 节点磁盘使用率（%） 	| 磁盘使用率过高会导致数据无法正常写入 |
| 节点HeapMemory使用率（%） |数值过高时影响查询性能 |