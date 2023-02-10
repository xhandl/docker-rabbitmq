# RabbitMQ
### Run and go Docker setup for RabbitMQ.

<br />

To start RabbitMQ on background via Docker just type:
```
docker compose up -d
```

Main parametrs can be modified via `.env` file.


Default configuration:
```
IMAGE: rabbitmq:3.11.8-management
CONTAINER NAME: rabbitmq
USER: admin
PASSWORD: admin
PORT: 5672 (default for RabbitMQ service)
      15672 (default for RabbitMQ web administration)
```

Data are persisted locally:
```
./volumes/rabbitmq/mnesia
```

Access to web administration: http://localhost:15672

Docker network:
```
rabbitmq
```