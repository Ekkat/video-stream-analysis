# Video Stream Processor
Video Stream Processor process kafka JSON messages. It uses OpenCV library for motion detection. This project requires following tools and technologies.

- JDK - 1.8
- Maven - 3.3.9
- ZooKeeper - 3.4.8
- Kafka - 2.11-0.10.2.0
- OpenCV - 3.2.0
- Spark - 2.1.1

Please check src/main/resources/stream-processor.properties for configuration details.

Run "mvn clean" command to install opencv-320.jar in local maven repository. Now you can execute below command to start the VideoStreamProcessor.

```sh
mvn clean package exec:java -Dexec.mainClass="com.iot.video.app.spark.processor.VideoStreamProcessor"
```
