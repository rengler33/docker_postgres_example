# docker_postgres_example
When you need a postgres database container on linux

Instructions:

`cp .env.example .env`

^ update as desired

`docker compose up`

From another terminal you can connect with:

`psql postgresql://postgres:postgres@localhost:5433/postgres`

^ adjust user:pass and db name as needed according to `.env` file


Notes: 

The biggest hangup was realizing I can't use port 5432, so that's why it's mapped to 5433.

This makes it easy to connect from outside the container using psql client.
