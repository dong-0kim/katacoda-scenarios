Kafka를 설치해 봅시다!

## Task

This is an _example_ of creating a scenario and running a **command**

`echo 'Hello World'`{{execute}}


1. `apt-get update`{{execute}}
2. `apt-get install telnet`{{execute}}
3. apt-get --assume-yes install default-jre{{execute}}
4. apt-get --assume-yes install zookeeperd{{execute}}
5. service zookeeper stop{{execute}}
6. mkdir $HOME/kafka{{execute}}
7. cd $HOME/kafka{{execute}}
8. wget http://www-us.apache.org/dist/kafka/2.5.0/kafka_2.12-2.5.0.tgz{{execute}}
9. mv *.tgz  kafka.tgz{{execute}}
10. tar -xvzf ./kafka.tgz --strip 1{{execute}}
11. rm kafka.tgz{{execute}}
