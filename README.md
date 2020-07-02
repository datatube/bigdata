# BigData

# 一.存储框架篇
## Hdfs
- Hdfs NameNode高可用如何实现，需要哪些角色
- Hdfs元数据管理流程？短时间大量小文件造成的nameNode宕机如何解决？
- Hdfs中edits-log和fsimage各自的作用是啥？
- Hdfs文件上传过程？在文件上传过程中如何建立数据管道？在建立数据管道过程中发生错误怎么进行容错处理？在数据传输过程中发生错误怎么进行容错处理？
- Hdfs文件下载过程？
- 简单说说Hdfs如何实现短路读

## HBase
- HBase的元数据.meta表rowKey是由什么组成的，value存储的是什么信息？.meta表只存在一台RegionServer会不会造成热点问题？
- HBase的一个region由哪些东西组成，RegionServer宕机之后如何感知，如何迁移数据
- HBase的数据在Hdfs上是怎么存储的，为什么HBase适合写多读少的业务
- HLog的数据在Hdfs上是怎么存储的？以及如何做过期处理？
- 写流程，HLog写入失败了怎么办，如果Region挂了怎么办，怎么恢复呢？MemoStore刷不到HFile里怎么办？
- MemStore的底层数据结构是啥？以及是怎么解决大量对象写入造成的内存碎片问题？
- 读流程，如何根据rowKey找到对应的RegionServer？以及是如何定位哪些HFile不存在目标rowkey？
- Hbase Compaction的原理？什么时候会触发Compaction?
- 使用bulkLoad为何能大大提高Hbase写入性能？原理是什么？
- 说说你们rowKey的设计


## Kafka
- Kafka是如何基于zk做元数据管理的？消费者偏移量offset写入zk会有啥问题？
- 简单说说Kafka Producer是如何基于os pagecache和磁盘顺序写实现高性能写入broker？
- Kafka Consumer是如何实现零拷贝？如果数据量远大于消费速度还会走零拷贝吗？
- Kafka的数据存储结构是什么样的？都有哪些索引？
- ISR机制是如何实现数据的高可用以及数据的一致性？
- Kafka如何保证数据不丢失？数据不重复？

# 二.计算框架篇
## Spark
- RDD、DataSet、DataFrame有什么区别，都有哪些特点
- 如果一个task执行比较慢，怎么解决，一定是数据倾斜么？
- Kafka与SparkStreaming集成，如何保证exactly once语义
- 大表 join 小表的优化方法，shuffle调优方法
- Spark的内存模型是怎样的
- Spark提交一个任务的执行过程（DAGScheduler、job划分、stage划分、task生成、资源调度、shuffle详细过程及各版本的演化）
- 需要关注自己服务的数据量、使用资源、资源设置依据，是否还可以减少，怎么测试
## Flink


## Zookeeper
- 什么是CAP协议
- 如何用Zookeeper实现分布式锁？使用redis或数据库呢

## Yarn
- Yarn有哪些组件，如何分配资源
## Hive
## SystemDesign
##
