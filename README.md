About postgres:
Enter docker:                   docker exec -it $id /bin/bash
                                docker exec -it go-rest-db-pg /bin/bash
Enter psql for database:        docker exec -it $id psql -d go-rest-postgresql -U admin
                                docker exec -it go-rest-postgresql psql -d go-rest-postgresql -p 5432 -h 127.0.0.1 -U admin

Entering in dtabase: useful commands
List of databases               \l
Enter database                  \c go-rest-postgresql
List tables in database         \dt

PGDATA directory                PGDATA: /var/lib/postgresql/data 

Having persistent data for postgresql
    Create a volume:
        docker volume create --name postgresql-volume -d local
    Run:
        docker-compose -f docker-compose-pers.yml up -d --build
---------------------------------------
For Dockerfile app
Enter bash: docker exec -it go-rest-pg /bin/bash       