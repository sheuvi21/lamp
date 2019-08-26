FROM php:7.3-apache

RUN docker-php-ext-install pdo pdo_mysql mysqli

RUN apt-get update && apt-get install -y msmtp
RUN echo 'sendmail_path = /usr/bin/msmtp -t' >> $PHP_INI_DIR/php.ini
