FROM php:7.2-apache 

  

COPY ./amp/ /var/www/html/ 

  
RUN apt-get update

RUN apt-get install iputils-ping curl vim -y

RUN docker-php-ext-install mysqli pdo pdo_mysql  

  

EXPOSE 80
