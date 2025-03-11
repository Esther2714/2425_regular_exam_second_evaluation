FROM php:8.2-apache
RUN docker-php-ext-install mysqli && docker-php-ext-enable mysqli
RUN apt-get update && apt-get upgrade -y
RUN rm -rf /var/www/*
ADD /home/ubuntu/ordinary/welcome.html var/www/html
RUN chown -R www-data:www-data /var/www/html
