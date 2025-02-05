# Database

## Docker Compose

Setup `.env` to contain these:

```sh
MYSQL_ROOT_PASSWORD=the_root_password
MYSQL_USER=the_user
MYSQL_PASSWORD=the_password
MYSQL_DATABASE=bandungdev
MYSQL_HOST_PORT=3306
MYSQL_CONTAINER_PORT=3306
```

Start Docker service.

Run Docker Compose up.

```sh
docker-compose up
```

If everything is fine, exit and run it again in detached mode.

```sh
docker-compose up -d
```

Push the schema to it.

```sh
pnpm db:push
```

Seed initial data

```sh
pnpm db:seed
```
