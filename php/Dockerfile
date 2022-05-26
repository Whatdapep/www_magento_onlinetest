FROM php:7.4-fpm-alpine

RUN docker-php-ext-install curl pdo mysqli sodium soap mbstring pdo_mysql 
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer