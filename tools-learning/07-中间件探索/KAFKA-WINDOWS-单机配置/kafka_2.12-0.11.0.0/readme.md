
#先启动kafka自带的zookeeper(当然这里也可以启动自己安装的zookeeper)
bin\windows\zookeeper-server-start.bat config\zookeeper.properties

#启动kafka服务
bin\windows\kafka-server-start.bat config\server.properties

#创建一个主题
bin\windows\kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic ARF

#创建一个消费者
bin\windows\kafka-console-consumer.bat --zookeeper localhost:2181 --topic ARF --from-beginning

#创建一个生产者
./kafka-console-producer.sh --broker-list localhost:9092 --topic ARF


bin\windows\zookeeper-server-start.bat config\zookeeper.properties