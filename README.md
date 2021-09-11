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

## Attributions/Credits

This configuration was originally forked from [khezen/compose-postgres](https://github.com/khezen/compose-postgres)