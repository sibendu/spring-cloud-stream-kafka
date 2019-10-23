Base code from this [repo][baserepo]

These event driven applications are built using Spring Boot and Spring Cloud Stream, eliminating no boilerplate messaging code.

## Step 1: 
Kafka or RabbitMQ can be run using docker-compose (start-server.sh), or local Kafka (runKafkaWindows.bat)

## Step 2:
Run LoanSource and LoanCheck microservices, run maven from respective folder: 
mvn clean package spring-boot:run -DskipTests=true -PKafka   
(or, to use profile -PActiveMQ) 


[baserepo]: https://github.com/benwilcock/spring-cloud-stream-demo.git
