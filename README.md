# tutorial-8-publisher

## Reflection 1a
Since there are 5 `publish_event` method calls within the `main` function inside src/main.rs, there would be 5 * `UserCreatedEventMessage` struct size.

## Reflection 1b
It means that both the subscriber and the publisher interact with the message broker at the same host and port using the same credentials (username and password) and protocol (amqp).
