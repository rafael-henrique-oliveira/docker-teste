FROM ubuntu

MAINTAINER Rafael Oliveira <rafaelhenrique.oliveira7@gmail.com>

RUN apt-get update

RUN apt-get install -y nginx

ADD exemplo /etc/nginx/sites-enabled/default

EXPOSE 8080
