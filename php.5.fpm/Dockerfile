FROM php:php:5.6-fpm
RUN apt-get update
RUN apt-get install -y libmcrypt-dev libpng-dev
RUN docker-php-ext-install mcrypt gd mysql iconv mysqli
RUN docker-php-ext-install pdo pdo_mysql pdo_mysqli
 
