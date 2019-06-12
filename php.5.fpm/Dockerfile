FROM php:5.6-fpm
RUN apt-get update
RUN apt-get install -y libmcrypt-dev libpng-dev libzip-dev 
RUN docker-php-ext-install mcrypt mysql iconv mysqli 
RUN docker-php-ext-install pdo pdo_mysql zip
RUN  apt-get install -y \
        libfreetype6-dev \
        libjpeg62-turbo-dev \
        libmcrypt-dev 
RUN docker-php-ext-configure gd --with-freetype-dir=/usr/include/ --with-jpeg-dir=/usr/include/ 
RUN docker-php-ext-install gd
