FROM php:7.4-apache

RUN docker-php-ext-install pdo_mysql

WORKDIR /var/www/html/

COPY ./src .
