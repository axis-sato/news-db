FROM mysql:8.0

COPY ./my.cnf /etc/mysql/conf.d/news.cnf
RUN cp -p /usr/share/zoneinfo/Japan /etc/localtime

EXPOSE 3306