FROM ubuntu
MAINTAINER leonardo@leonix.com

RUN apt update && apt install -y apache2 && apt clean && rm -rf /var/lib/apt/lists/*

ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache2
ENV APACHE_LOCK_DIR /var/lock/apache2
ENV APACHE_PID_FILE /var/run/apache2.pid

RUN mkdir -p $APACHE_RUN_DIR $APACHE_LOCK_DIR $APACHE_LOG_DIR

LABEL app minha_app

ADD index.html /var/www/html

VOLUME /var/www/html

WORKDIR /var/www/html

ENTRYPOINT ["/usr/sbin/apache2"]

CMD ["-D", "FOREGROUND"]

EXPOSE 80
