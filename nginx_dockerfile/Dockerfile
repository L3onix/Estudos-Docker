FROM ubuntu
MAINTAINER soueu@soueu.com

RUN apt update \
    && apt install -y nginx php-fpm\
    && apt clean

COPY index.html /var/www/html/

ENV jeferson lindo

VOLUME /var/www/html

CMD /usr/sbin/nginx -g 'daemon off;'

EXPOSE 80
