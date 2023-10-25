## Kafka Docker
This configuration uses the Confluent Kafka image and the Kafdrop image, 
which is a popular open-source web UI for managing Kafka clusters.

**Zookeeper:** Service uses the official Confluent Zookeeper image. <br />

**Kafka:** Service uses the official Confluent Kafka image. It depends on the Zookeeper service, and the necessary Kafka configuration for single-node development use is provided. You can adjust the configuration to suit your requirements. <br />

**Kafdrop:** Service uses the Kafdrop image for the Kafka web UI. It's configured to connect to the Kafka broker on kafka:9092, which matches the name of the Kafka service in the Docker Compose file.

```bash
docker-compose up -d && docker-compose up
```
