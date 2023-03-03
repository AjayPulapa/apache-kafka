Start Zookeeper Server:
-----------------------------
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties

D:\kafka_2.13-2.8.1\bin\windows>zookeeper-server-start.bat D:\kafka_2.13-2.8.1\config\zookeeper.properties 

Kafka Server:
------------------------
.\bin\windows\kafka-server-start.bat .\config\server.properties

D:\kafka_2.13-2.8.1\bin\windows>kafka-server-start.bat D:\kafka_2.13-2.8.1\config\server.properties

Consume the Data Via Console:
---------------------------------
.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic ajaypulapa --from-beginning

Create Topic:
-----------------------------------
Kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic ajaypulapa

List of Topics:
-------------------------------
Kafka-topics.bat --list --zookeeper localhost:2181


Referred WebSites:
----------------------------
https://www.javainuse.com/spring/spring-boot-apache-kafka-hello-world
https://www.javaguides.net/2022/05/spring-boot-kafka-producer-consumer-example-tutorial.html