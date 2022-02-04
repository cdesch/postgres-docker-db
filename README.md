# postgres-docker-db

A [PostgreSQL](https://www.postgresql.org/) DB and [PGAdmin](https://www.pgadmin.org/) setup using [Docker](https://www.docker.com/) contianers with [Docker Compose](https://docs.docker.com/compose/)

## Run

Start the project to run the database

    docker-compose up

Start Detached

    docker-compose up -d

## Configuration

DB Connection

    username: postgres
    password: postgres
    port:     5432
    hostname: localhost

## MongoDB

   docker-compose -f docker-compose-mongodb.yaml

## CockRoachDB

   docker-compose -f docker-compose-crdb.yaml
   docker exec -it $(docker-compose ps -q roach1) /bin/sh
   docker run --network=postgres-docker-db_ -it cockroachdb/cockroach:latest init --insecure --host=roach1:26257

## Attributions/Credits

This configuration was originally forked from [khezen/compose-postgres](https://github.com/khezen/compose-postgres)
