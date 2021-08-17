Kafka를 설치해 봅시다!

## Task

Kafka와 Zookeeper를 설치해 봅시다.

1. `apt-get update`{{execute}}
2. `apt-get --assume-yes install default-jre`{{execute}}
3. `apt-get --assume-yes install zookeeperd`{{execute}}
4. `service zookeeper stop`{{execute}}
5. `mkdir kafka`{{execute}}
6. `cd $HOME/kafka`{{execute}}
7. `wget https://mirror.navercorp.com/apache/kafka/2.7.1/kafka_2.13-2.7.1.tgz`{{execute}}
8. `mv *.tgz  kafka.tgz`{{execute}}
9. `tar -xvzf ./kafka.tgz --strip 1`{{execute}}
10. `rm kafka.tgz`{{execute}}
11. `vi config/server.properties`{{execute}}
12. `service zookeeper start`{{execute}}
13. `nohup $HOME/kafka/bin/kafka-server-start.sh $HOME/kafka/config/server.properties > $HOME/kafka.log 2>&1 &`{{execute}}
