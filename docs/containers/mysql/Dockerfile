FROM mysql:9.0.1

COPY mysqld.cnf /etc/mysql/mysql.conf.d/mysqld.cnf
COPY init.sql /docker-entrypoint-initdb.d/init.sql
