topic, producer, consumer 실습해 봅시다!

## Task

topic, producer, consumer 실습

15. `./kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 3 --topic test`

16. `./kafka-console-producer.sh --bootstrap-server localhost:9092 --topic test`

17. `./kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test --from-beginning`
18. `./kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test -group testgroup --from-beginning`

19. `./kafka-consumer-groups.sh --bootstrap-server localhost:9092 --list`
20. `./kafka-consumer-groups.sh --bootstrap-server localhost:9092 --group testgroup --describe`
21. `./kafka-consumer-groups.sh --bootstrap-server localhost:9092 --group testgroup --topic test --reset-offsets --to-earliest --execute`
22. `./kafka-consumer-groups.sh --bootstrap-server localhost:9092 --group testgroup --topic test:1 --reset-offsets --to-offset 10 --execute`

