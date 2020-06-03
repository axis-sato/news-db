FROM mysql:8.0

RUN cp -p /usr/share/zoneinfo/Japan /etc/localtime

USER mysql

COPY ./my.cnf /etc/mysql/conf.d/news.cnf

EXPOSE 3306