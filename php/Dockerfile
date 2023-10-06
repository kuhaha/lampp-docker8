FROM php:8.1-apache 
RUN apt-get update && apt-get install -y libonig-dev && docker-php-ext-install pdo_mysql mysqli mbstring
COPY --from=composer /usr/bin/composer /usr/bin/composer
