# tutorial-8-publisher

## Reflection 1a
Since there are 5 `publish_event` method calls within the `main` function inside src/main.rs, there would be 5 * `UserCreatedEventMessage` struct size.

## Reflection 1b
It means that both the subscriber and the publisher interact with the message broker at the same host and port using the same credentials (username and password) and protocol (amqp).

![rabbitmq_1.jpeg](assets/rabbitmq_1.jpeg)

The image above shows the RabbitMQ dashboard, specifically the Overview tab. The Overview tab displays the amount of queued messages from the last minute, message rates per second, global counts, RabbitMQ nodes, and more.

![rabbitmq_2.jpeg](assets/rabbitmq_2.jpeg)

The image above shows the RabbitMQ dashboard after receiving a connection from the publisher app.

![rabbitmq_3.png](assets/rabbitmq_3.png)

The image above shows the RabbitMQ dashboard, the publisher app's console and the subscriber app's console. After we invoke `cargo run` on the publisher console, the publisher's app sends 5 messages to RabbitMQ. RabbitMQ then forwards the messages to the subscriber's app, notifying the subscriber to log the messages to the console.
