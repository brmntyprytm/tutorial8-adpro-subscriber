### Tutorial 8

#### Bramantyo Priyo Utomo - 2206821563

1. AMQP stands for Advanced Message Queuing Protocol. It's an open standard for message-oriented middleware, primarily used for exchanging messages between applications or systems. AMQP provides a framework for queuing, routing, and delivering messages between applications in a reliable, secure, and efficient manner. It's designed to facilitate communication between diverse platforms and programming languages, making it a popular choice for building distributed systems, messaging systems, and enterprise application integration (EAI) solutions.

2. `amqp://guest:guest@localhost:5672` is a URI (Uniform Resource Identifier) that specifies the connection parameters for an AMQP (Advanced Message Queuing Protocol) broker. The first "guest" is the username for authentication. The second "guest" is the password for authentication. `localhost:5672` is the hostname and port of the AMQP broker. This URI is passed to the `CrosstownBus::new_queue_listener()` method to create a new listener for consuming messages from a specific queue in the AMQP broker.

#### Simulate slow requests

- These screenshot shows the console output of the publisher program. Five events were successfully sent to the message broker with sleep 10 ms.

- Subscriber
  ![img2](assets/iamges/RabbitMQ.png)

#### 3 Subscribers 1 Publisher

![img3](assets/iamges/3sub1pub.png)
![img4](assets/iamges/3sub1pubrab.png)

- The screenshot above shows the console output of the subscriber program. It demonstrates the successful consumption and processing of the five events sent by the publisher program. Each event contains information about a user creation event, including the user ID and user name.

The subscriber program handles each received message by printing it to the console. This output confirms that the subscriber is effectively receiving and processing messages from the message broker.
