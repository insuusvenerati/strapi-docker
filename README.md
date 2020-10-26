# Strapi Docker


# Environment

## Mongo

```yaml
environment:
  MONGODB_USERNAME: ${DATABASE_USERNAME}
  MONGODB_PASSWORD: ${DATABASE_PASSWORD}
  MONGODB_DATABASE: ${DATABASE_NAME}
```

## Strapi

```yaml
environment:
  NODE_ENV: production
  DATABASE_CLIENT: mongo
  DATABASE_HOST: db
  DATABASE_PORT: 27017
  DATABASE_NAME: ${DATABASE_NAME}
  DATABASE_USERNAME: ${DATABASE_USERNAME}
  DATABASE_PASSWORD: ${DATABASE_PASSWORD}
```

<!-- # Get started

## Setup

Install docker https://docs.docker.com/engine/install/ubuntu/ and docker-compose

`git clone https://github.com/insuusvenerati/strapi-docker`

Create a `.env` file from `.env-sample` and fill in the empty fields.

Create a folder called `app` for Strapi to live in.

`docker-compose up -d` to start the services.

> Monitor logs with `docker-compose logs -f` -->