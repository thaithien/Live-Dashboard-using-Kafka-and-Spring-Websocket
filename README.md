# Live-Dashboard-using-Kafka-and-Spring-Websocket

This Demo application reads data from Apache Kafka topic and updating the View using Spring Websocket on real-time.

Check the working Video : https://www.youtube.com/watch?v=GD0t-LwVRIM
Check the Tutorial : https://dzone.com/articles/live-dashboard-using-apache-kafka-and-spring-webso

## How to run

- start docker : `docker-compose -f docker-compose.yaml up -d`
- connect to docker `docker exec -it kafka1 /bin/bash`
- create a topics `kafka-topics.sh --bootstrap-server localhost:9092 --topic livetemperature --create --partitions 3 --replication-factor 1`

## Start java application

mvn spring-boot:run

## Produce data 
`kafka-console-producer --broker-list localhost:9092 --topic livetemperature`


