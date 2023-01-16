# docker_postgres_example
When you need a postgres database container on linux

The biggest hangup was realizing I can't use port 5432, so that's why it's mapped to 5433.

This makes it easy to connect from outside the container using psql client.
