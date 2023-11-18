# Kafka IBM Real Time Stocking

## Dataset

In this project, we will use this dataset:
[https://www.kaggle.com/datasets/bhanuprasanna527/stock-market-prediction](https://www.kaggle.com/datasets/bhanuprasanna527/stock-market-prediction)

## Install Environment

- install kafka ```wget https://downloads.apache.org/kafka/3.3.1/kafka_2.12-3.3.1.tgz```
- extract kafka ```tar -xvf kafka_2.12-3.3.1.tgz```
- install java jdk 1.8.0 (set environment for JAVA_HOME)


## Start Kafka Server

- cd kafka_2.12-3.3.1
- Start Zookeeper: bin/zookeeper-server-start.sh config/zookeeper.properties
- Start Broker: bin/kafka-server-start.sh config/server.properties
- Create Topic: bin/kafka-topics.sh --create --topic demo_kafka --bootstrap-server localhost:9092
- To see Topic's lists:  bin/kafka-topics.sh --bootstrap-server localhost:9092 --list
- Start Producer: bin/kafka-console-producer.sh --topic demo_kafka --bootstrap-server localhost:9092
- Start Consumer: bin/kafka-console-consumer.sh --topic demo_kafka --bootstrap-server localhost:9092

## How to use

- clone this github ```git clone ```
- install all libraries ```pip install -r requirements.txt```
- run all shell in **kafka_consumer.ipynb** and **kafka_producer.ipynb**
