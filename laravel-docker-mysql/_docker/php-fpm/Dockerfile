FROM php:7.4-fpm

WORKDIR /var/www

RUN apt-get update && apt-get install -y \
autoconf build-essential \
git \
zip \
unzip

RUN apt-get clean && rm -rf /var/lib/apt/lists/*

COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

RUN usermod -u 1000 -d /home/www-data www-data
RUN mkdir -p /home/www-data/.composer && \
    chown -R www-data:www-data /home/www-data

USER www-data
