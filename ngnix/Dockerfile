FROM php:8.0-fpm-buster
WORKDIR /var/www
RUN docker-php-ext-install pdo pdo_mysql
ADD . /var/www
RUN chown -R www-data:www-data /var/www
RUN chmod 755 /var/www