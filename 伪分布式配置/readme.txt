注意:
这里的思想是用localhost作为slave
使用hostname(ubuntu)作为master
并且需要下面两个启动
$HADOOP/sbin/start-all.sh
$SPARK_HOME/sbin/start-all.sh
--------------------------------------------------------------------------------
jps效果是:
8050 Master
4498 NameNode
4611 DataNode
8133 Worker
5112 NodeManager
5002 ResourceManager
9358 Jps
--------------------------------------------------------------------------------
验证方法是:
spark-shell --master spark://ubuntu:7077
