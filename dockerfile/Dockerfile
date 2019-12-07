FROM debian:9

RUN apt-get update

RUN apt-get install apache2

RUN echo "welcome" >> /var/www/html/index.html

COPY ./var/www/html

RUN service apache2 start 

CMD tail -f /var/log/apache2/access.log
