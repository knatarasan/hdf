# Quick start guide

## 1.Create a topic

/usr/hdp/current/kafka-broker/bin/kafka-topics.sh --create --zookeeper cent7-gra02.field.hortonworks.com:2181 --replication-factor 1 --partitions 1 --topic test

/usr/hdp/current/kafka-broker/bin/kafka-topics.sh --list --zookeeper cent7-gra02.field.hortonworks.com:2181


## Send some message

/usr/hdp/current/kafka-broker/bin/kafka-console-producer.sh --broker-list cent7-gra03.field.hortonworks.com:6667 --topic test


## Start a consumer

/usr/hdp/current/kafka-broker/bin/kafka-console-consumer.sh --bootstrap-server cent7-gra03.field.hortonworks.com:6667 --topic test --from-beginning


