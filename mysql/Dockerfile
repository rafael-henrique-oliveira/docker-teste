FROM ubuntu

MAINTAINER Rafael Oliveira <rafaelhenrique.oliveira7@gmail.com>

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update -qq && apt-get install -y mysql-server-5.5

ADD my.cnf /etc/mysql/conf.d/my.cnf

RUN chmod 664 /etc/mysql/conf.d/my.cnf

ADD run /usr/local/bin/run

RUN chmod +x /usr/local/bin/run

VOLUME ["/var/lib/mysql"]

EXPOSE 3306

CMD ["/usr/local/bin/run"]
