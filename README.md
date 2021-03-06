# Laravel-docker-custom

Easier to access boilerplate to run laravel on docker. To run you will need [docker](https://docs.docker.com/engine/install/) and [docker-compose](https://docs.docker.com/compose/install/) installed on your computer. [Bitnami official docker documentation](https://hub.docker.com/r/bitnami/laravel).

## Bitnami
To initialize the image run
```
docker-compose up -d
```
To run artisan commands
```
docker-compose exec myapp php artisan <command>
```
To stop the application run
```
docker-compose down
```

## Ngnix
To build the first time run
```
docker-compose build && docker-compose up -d
```
After building the first time you can run
```
docker-compose up -d
```
To run artisan commands
```
docker-compose exec php php /var/www/html/artisan <command>
```
To stop the application run
```
docker-compose down
```
You will need to initialize a laravel application in the src dir with the default composer laravel command
