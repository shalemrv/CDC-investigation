CDC - Investigation

https://medium.com/blablacar/streaming-data-out-of-the-monolith-building-a-highly-reliable-cdc-stack-d71599131acb

Findings

1. Debezium cannot work without Kafka
2. Debezium will publish CDC events to Kafka and another custom or any integration tool can be used as a bridge component to Consume Kafka events and re-publish to RabbitMQ


## `Final` Debezium RabbitMQ sink connector  - DRSC (Not an official abbreviation)

Debezium can be used with RabbitMQ without Kafka using DRSC

This way, RabbitMQ can consume the change events directly from Debezium (instead of any bridge components)

https://debezium.io/blog/2023/04/03/debezium-2-2-beta1-released/


PostgreSQL to RabbitMQ CDC using Debezium Server
https://blog.devops.dev/postgresql-to-rabbitmq-cdc-using-debezium-server-5c7c70de8afd
This can be tweaked for a MySQL source

