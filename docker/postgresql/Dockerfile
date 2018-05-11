FROM postgres:10.3

COPY postgresql.conf /usr/lib/postgresql/postgresql.conf
CMD ["-c", "config_file=/usr/lib/postgresql/postgresql.conf"]

#COPY postgresql.conf /postgresql.conf
#COPY set-config.sh /docker-entrypoint-initdb.d/set-config.sh

#COPY postgresql.conf /var/lib/postgresql/data/postgresql.conf
