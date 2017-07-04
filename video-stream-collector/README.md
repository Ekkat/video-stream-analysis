# Video Stream Collector
Video Stream Collector converts video file or webcam feed to JSON messages and send to Kafka. This project requires following tools and technologies.

- JDK - 1.8
- Maven - 3.3.9
- ZooKeeper - 3.4.8
- Kafka - 2.11-0.10.2.0
- OpenCV - 3.2.0

Please check src/main/resources/stream-collector.properties for configuration details.

Run "mvn clean" command to install opencv-320.jar in local maven repository. Now you can execute below command to start the VideoStreamCollector.

```sh
mvn clean package exec:java -Dexec.mainClass="com.iot.video.app.kafka.collector.VideoStreamCollector"
```
