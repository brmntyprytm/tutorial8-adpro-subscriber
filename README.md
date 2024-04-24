### Tutorial 8

#### Bramantyo Priyo Utomo - 2206821563

1. AMQP stands for Advanced Message Queuing Protocol. It's an open standard for message-oriented middleware, primarily used for exchanging messages between applications or systems. AMQP provides a framework for queuing, routing, and delivering messages between applications in a reliable, secure, and efficient manner. It's designed to facilitate communication between diverse platforms and programming languages, making it a popular choice for building distributed systems, messaging systems, and enterprise application integration (EAI) solutions.

2. `amqp://guest:guest@localhost:5672` is a URI (Uniform Resource Identifier) that specifies the connection parameters for an AMQP (Advanced Message Queuing Protocol) broker. The first "guest" is the username for authentication. The second "guest" is the password for authentication. `localhost:5672` is the hostname and port of the AMQP broker. This URI is passed to the `CrosstownBus::new_queue_listener()` method to create a new listener for consuming messages from a specific queue in the AMQP broker.
