# Laravel Docker Mongodb

This is a simple [Laravel](https://laravel.com/docs/8.x) application created
with [Composer](https://getcomposer.org/download/)
using [Docker](https://www.docker.com/), using the command below:

`composer create-project laravel/laravel laravel-docker-mongodb`

The application has its necessary configurations in order to run with mongodb container as well.

## Requirements for building and running the application

- [Docker](https://docs.docker.com/get-docker/)

## Application Build and Run

After cloning the repository get into the laravel-docker-mongodb directory and run:

`docker-compose up -d`

`docker-compose exec php-fpm composer install`

`docker-compose exec php-fpm cp .env.example .env`

## Then finally test the application

Go to [http://localhost:8000](http://localhost:8000) in order to see the application running.
