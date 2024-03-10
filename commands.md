Инициализация зависимостей

```
go mod init github.com/EvgeniyBudaev/microservices-in-go/front-end
go mod init github.com/EvgeniyBudaev/microservices-in-go/broker-service
go mod init github.com/EvgeniyBudaev/microservices-in-go/listener-service
go mod init github.com/EvgeniyBudaev/microservices-in-go/authentication-service
go mod init github.com/EvgeniyBudaev/microservices-in-go/logger-service
go mod init github.com/EvgeniyBudaev/microservices-in-go/mail-service
```

Chi
```
go get github.com/go-chi/chi/v5
go get github.com/go-chi/chi/middleware
go get github.com/go-chi/cors
```

Docker
из /infra
```
docker-compose up -d
```
появится контейнер в docker desktop
```
docker-compose down
```

Make
```
make stop
make down
make up_build
make down
make start
```

Запуск RabbitMQ
```
docker-compose up
```
15672 - порт админки
5672 - порт RabbitMQ
После запуска можем перейти в админку по адресу http://localhost:15672

https://github.com/rabbitmq/rabbitmq-tutorials/tree/main/go
```
go get github.com/rabbitmq/amqp091-go
```

Crypto
```
go get golang.org/x/crypto
```

SQL
```
go get github.com/jackc/pgconn
go get github.com/jackc/pgx/v4
go get github.com/jackc/pgx/v4/stdlib
```

Toolbox
```
go get -u github.com/tsawler/toolbox
```

Mongo
Crypto
```
go get go.mongodb.org/mongo-driver/mongo
go get go.mongodb.org/mongo-driver/mongo/options
```

Mail
```
go get github.com/vanng822/go-premailer/premailer
go get github.com/xhit/go-simple-mail/v2
```