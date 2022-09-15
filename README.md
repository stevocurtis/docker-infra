# docker-infra

To start mongo db with express server run:

`docker-compose -f mongo/mongo-compose.yml up -d`

To start rabbitmq run:

`docker-compose -f rabbitmq/rabbitmq-compose.yml up -d`

To login to the rabbitmq manangement console go to http://127.0.0.1:15672/ as guest/guest

To start mysql run:

`docker-compose -f mysql/mysql-compose.yml up -d`