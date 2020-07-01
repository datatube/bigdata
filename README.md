# BigData
## Hadoop(Hdfs/Yarn)
- Hdfs NameNode高可用如何实现，需要哪些角色
- Yarn有哪些组件，如何分配资源
## Spark
- RDD、DataSet、DataFrame有什么区别，都有哪些特点
- 如果一个task执行比较慢，怎么解决，一定是数据倾斜么？
- Kafka与SparkStreaming集成，如何保证exactly once语义
- 大表 join 小表的优化方法，shuffle调优方法
- Spark的内存模型是怎样的
- Spark提交一个任务的执行过程（DAGScheduler、job划分、stage划分、task生成、资源调度、shuffle详细过程及各版本的演化）
- 需要关注自己服务的数据量、使用资源、资源设置依据，是否还可以减少，怎么测试
## Flink
## Kafka
## Zookeeper
- 什么是CAP协议
- 如何用Zookeeper实现分布式锁？使用redis或数据库呢
## HBase
- HBase的数据在Hdfs上是怎么存储的，为什么HBase适合写多读少的业务
- 读写流程，HLog写入失败了怎么办，如果Region挂了怎么办，怎么恢复呢？MemoStore刷不到HFile里怎么办？
- HBase的一个region由哪些东西组成，RegionServer宕机之后如何感知，如何迁移数据
## Hive
## SystemDesign
###
