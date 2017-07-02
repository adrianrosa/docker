FROM php:7.0-apache

RUN docker-php-ext-install mysqli
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/bin/ && mv /usr/bin/composer.phar /usr/bin/composer

COPY 000-default.conf /etc/apache2/sites-available/000-default.conf

EXPOSE 80
EXPOSE 443
