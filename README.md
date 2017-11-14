modified from https://github.com/howtoprogram/Apache-Kafka-Tutorials
"# Apache-Kafka-Tutorials"

## 1. Import source code into Eclipse

Menu **File –> Import –> Maven –> Existing Maven Projects**

Browse to your source code location

Click **Finish** button to finish the importing

## 2. Run the application
1. Open command line in your Kafka installation folder
2. Launch Zookeeper with `.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties`
3. Open a second command line in your Kafka installation folder
4. Launch first Kafka broker: `.\bin\windows\kafka-server-start.bat .\config\server-1.properties`
5. Open a third command line in your Kafka installation folder
6. Launch second Kafka broker: `.\bin\windows\kafka-server-start.bat .\config\server-2.properties`
7. Open a fourth command line in your Kafka installation folder
8. Create a topic: `.\bin\windows\kafka-topics.bat --create --zookeeper localhost:2181 --replication-factor 2 --partitions 4 --topic kafkatest` 
9.Open the **ProducerTest.java** 

**Right click -> Run As -> Java Application** or use the shortcut: **Alt+Shift+x, j** to start the main method


10.Open the **ConsumerTest.java** 

**Right click -> Run As -> Java Application** or use the shortcut: **Alt+Shift+x, j** to start the main method

All the source code are described in: [Apache Kafka 0.9 Java Client API Example] (http://howtoprogram.xyz/2016/05/02/apache-kafka-0-9-java-client-api-example)

## 3. Related Posts

## [Getting started with Apache Kafka 0.9](http://howtoprogram.xyz/2016/04/30/getting-started-apache-kafka-0-9)
## [Create Multi-threaded Apache Kafka Consumer](http://howtoprogram.xyz/2016/05/29/create-multi-threaded-apache-kafka-consumer/) 

