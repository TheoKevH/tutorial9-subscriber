# Tutorial A: Subscriber

**Name**: Theodore Kevin Himawan

**NPM**: 2306210973

**Class**: Adpro A

## Reflection 1

> a. What is amqp?

<p align="justify">AMQP or Advanced Message Queuing Protocol is a protocol used for message-oriented middleware. It allows an application to communicate with the message broker that implements the protocol.</p>

> b. What does it mean? guest:guest@localhost:5672, what is the first guest, and what is the second guest, and what is localhost:5672 is for?

<p align="justify">That is an AMQP URI that is used to connect to a RabbitMQ server. The first guest is the username, while the second guest is the password. Localhost:5672 is the hostname where RabbitMQ is running (in this case is my local computer, in port 5672).</p>

## Simulating Slow Subscriber

![Queue](static/images/queue.png)

The total number of queue is because of the number of data sent by the publisher. Because the code is simulated to be slow, there are more requests to be processed by the slower subscriber than the publisher. All the unprocessed requests are put in the queue. In my computer, I got 15 queues. 