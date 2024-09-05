FROM mysql:5.7.24

COPY mysqld.cnf /etc/mysql/mysql.conf.d/mysqld.cnf
COPY init.sql /docker-entrypoint-initdb.d/init.sql
