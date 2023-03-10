I'm sorry, but I cannot generate images as I am a text-based program. However, I can describe the high-level architecture of a Kafka consumer API using the code we've been working with.

The Kafka consumer API is built using the Kafka client library, which provides a high-level interface for consuming messages from Kafka topics. The consumer API is typically a standalone application that connects to a Kafka cluster and subscribes to one or more topics to consume messages from.

The high-level architecture of a Kafka consumer API can be represented as follows:


```
                    +----------------+
                    | Kafka Producers|
                    +----------------+
                           \|/
                            |
                     +--------------+
                     | Kafka Cluster|
                     +--------------+
                            |
                           /|\
                    +----------------+
                    | Kafka Consumers|
                    +----------------+
                            |
                            |
                   +------------------+
                   | Apps - Business  |
                   +------------------+

```


A simple Kafka consumer API

Just replace to your environment:
```java
TOPIC_NAME = "my_topic";
BOOTSTRAP_SERVERS = "localhost:9092";
GROUP_ID = "my_group";
keepPolling = true;
```
