FROM mysql:latest
COPY ./my.cnf /etc/mysql/my.cnf
ADD ./init_db.sh /tmp/init_db.sh
RUN /tmp/init_db.sh