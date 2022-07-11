
## How to install Kafka on Mac 

#### Run brew install
```
brew install kafka
```


#### Start ZooKeeper 
```
zookeeper-server-start /usr/local/etc/kafka/zookeeper.properties
```

#### Start your Kafka Server
```
kafka-server-start /usr/local/etc/kafka/server.properties
```

#### Find your Kafka Logs at: 
```
/usr/local/var/lib/kafka-logs
```


#### Create new topic:
``` 
cd /usr/local/Cellar/kafka/3.2.0/libexec/bin
./kafka-topics.sh --create --topic demo --bootstrap-server localhost:9092
```


#### Describe the topic you created
```
./kafka-topics.sh --describe --topic demo --bootstrap-server localhost:9092
```

#### Add some data to your new topic 
```
./kafka-console-producer.sh --topic demo --bootstrap-server localhost:9092
```


#### Read the data from your new topic
```
./kafka-console-consumer.sh --topic demo --from-beginning --bootstrap-server localhost:9092
```


#### Install Offset Explorer 2 

[Download Offset Explorer](https://www.kafkatool.com/download.html)


