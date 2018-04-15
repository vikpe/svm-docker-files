FROM php:7.2-fpm

RUN apt-get update && apt-get install -y nano procps

RUN docker-php-ext-install -j$(nproc) iconv mysqli

COPY php.ini /usr/local/etc/php/conf.d/svm.php.ini
