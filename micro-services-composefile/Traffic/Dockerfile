FROM ubuntu:latest

LABEL TODO="file"

RUN apt update

RUN apt install apache2 -y

RUN rm -rf /var/www/html/*

WORKDIR /var/www/html/

RUN mkdir /var/www/html/traffic

COPY ./ /var/www/html/traffic/

EXPOSE 81
    
CMD ["apachectl", "-D", "FOREGROUND"]
