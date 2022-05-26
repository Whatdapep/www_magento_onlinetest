FROM php:7.4-fpm-alpine

RUN docker-php-ext-install curl pdo mysqli sodium soap mbstring pdo_mysql 
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer
# 
RUN find var generated vendor pub/static pub/media app/etc -type f -exec chmod g+w {} +
#
RUN find var generated vendor pub/static pub/media app/etc -type f -exec chmod g+w {} +
#########chown -R :www-data . # Ubuntu
RUN chown -R :www-data . # Ubuntu
#
RUN chmod u+x bin/magento
#
RUN ln -s /etc/nginx/sites-available/magento /etc/nginx/sites-enabled




