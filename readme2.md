
Representational state transfer   is the  software architecture used for web services. RESTful web services provides  computer systems and internet work together.
According to rest api clients and servers are separated from each other. Server doesnt keep any information about the client so its stateless.
They have uniform interface and are loosely coupled, like the way we want in microservices. They have a layered system.They can also extend the functionality of client temporarly on demand.
A RESTful web application provides information about its resources. Resources are identified with the help of URLs.

But what is the best serialization technology and how are we going to decide.
If we have already started with  protocol buffers we should go on with that . Or if we are using json we should go on with that MessagePack should be considered here for optimization.
Avro should be used if we are dealing with big data.

The companies using the technology are:
Facebook, Cassandra project  Apache Thrift
Google,  ActiveMQ Protocol Buffers
Avro Apache Hadoop
Protocol Buffers have a better documentation when compared with Apache Thrift. Protocol Buffers are slightly faster. 
Avro does not require that code be generated. Data is always accompanied by a schema that permits full processing of that data without
code generation, static datatypes, etc.
In Avro serialisation and deserialization can be done without code generation. Also code generation is also available for statically typed languages such as java 




There is a Benchmarking for thrift-protobuf-Avro and you get get the document from [Benchmark](https://code.google.com/archive/p/thrift-protobuf-compare/wikis/BenchmarkingV2.wiki)

<p align="center">
  <img  src="https://github.com/okansungur/Articles/blob/main/Create_object_serialize_deserialize.png"><br/>
 
</p>


![This is an image]()

Total Time 
Create an object, serialize it to a byte array, then deserialize it back to an object. 







