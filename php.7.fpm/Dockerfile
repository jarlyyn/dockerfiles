FROM php:7-fpm
RUN apt-get update
RUN apt-get install -y libpng-dev libzip-dev
RUN docker-php-ext-install iconv mysqli zip 
RUN docker-php-ext-install pdo pdo_mysql
RUN  apt-get install -y \
        libfreetype6-dev \
        libjpeg62-turbo-dev 
RUN docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ 
RUN docker-php-ext-install gd
