# Laravel Docker Mysql

This is a simple [Laravel](https://laravel.com/docs/8.x) application created
with [Composer](https://getcomposer.org/download/)
using [Docker](https://www.docker.com/), using the command below:

`composer create-project laravel/laravel laravel-docker-mysql`

The application has its necessary configurations in order to run with mysql container as well.

## Requirements for building and running the application

- [Docker](https://docs.docker.com/get-docker/)

## Application Build and Run

After cloning the repository get into the laravel-docker-mysql directory and run:

`cp .env.example .env`

`docker-compose up -d`

`docker-compose exec php-fpm composer install`

## Then finally test the application

Go to [http://localhost:8000](http://localhost:8000) in order to see the application running.
