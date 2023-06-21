### Architectural messaging patterns
 
##### Message exchange architectures
###### Pub-Sub
The Pub-Sub pattern is one in which a publisher sends a message to a topic on a message broker. You can think of a topic as an inbox. The concept of an inbox has different names according to the implementation technology. For example, * *RabbitMQ calls the inbox an Exchange while Kafka calls the inbox a Topic*. A subscriber binds to the topic and receives messages from the topic in an asynchronous manner.
