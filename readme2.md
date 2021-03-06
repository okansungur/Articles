## Serialization Technologies Rest, Avro,Thrift, Grpc , MessagePack   

**REST**: Representational state transfer   is the  software architecture used for web services. RESTful web services provides  computer systems and internet work together.
According to rest api clients and servers are separated from each other. Server doesnt keep any information about the client so its stateless.
They have uniform interface and are loosely coupled, like the way we want in microservices. They have a layered system.They can also extend the functionality of client temporarly on demand.
A RESTful web application provides information about its resources. Resources are identified with the help of URLs.

- For Apache Thrift please checkout [Apache Thrift and Spring Boot](https://okansungur.medium.com/apache-thrift-and-spring-boot-8af7fd3ccb09)
- For protocol buffers please checkout [GRPC Spring Boot Tutorial](https://okansungur.medium.com/grpc-springboot-tutorial-fbc0c0a60780)
- For  Apache Avro please checkout [Kafka, Apache Avro and Confluent Platform with Spring Boot](https://okansungur.medium.com/kafka-apache-avro-and-confluent-platform-with-spring-boot-ed86378e2d6b)
- For MessagePack please checkout [MessagePack Tutorial with Spring Boot](https://okansungur.medium.com/messagepack-tutorial-with-spring-boot-ed80c756b14d)


But what is the best serialization technology and how are we going to decide it?. It depends on our software.
If we have already started with  protocol buffers or Apache Thrift  we should go on with that . Or if we are using json we should go on with that, MessagePack can  be considered  for optimization here. Avro should be used if we are dealing with big data.

The companies using the technology are:
*Facebook, Cassandra project*  Apache Thrift
*Google,  ActiveMQ* Protocol Buffers
*Apache Hadoop* Avro 
Protocol Buffers have a better documentation when compared with Apache Thrift. Protocol Buffers are slightly faster. 
Avro does not require that code be generated. Data is always accompanied by a schema that permits full processing of that data without
code generation, static datatypes, etc.
In Avro serialisation and deserialization can be done without code generation. Also code generation is also available for statically typed languages such as java 


There is a Benchmarking for thrift-protobuf-Avro and you can get the document from [Benchmark](https://code.google.com/archive/p/thrift-protobuf-compare/wikis/BenchmarkingV2.wiki) There is also serialization and deserialization performances 


<p align="center">
  <img  src="https://github.com/okansungur/Articles/blob/main/Create_object_serialize_deserialize.png"><br/>
 
</p>











