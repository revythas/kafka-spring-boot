# SETUP kafka cluster
You can dowload kafka .tgz from here [https://kafka.apache.org/quickstart] 
 
- bin/zookeeper-server-start.sh config/zookeeper.properties

- bin/kafka-server-start.sh config/server.properties

- bin/kafka-topics.sh --list --zookeeper localhost:2181


# Test our codebase

- curl -X POST -F ‘message=test’ http://localhost:9000/kafka/publish
