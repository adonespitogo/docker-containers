# docker-services

Docker containers for common system services like databases.

I work on multiple enviroments like Mac OS and a variaty of linux operating systems. One of the common services I need to install in my local development machine are databases for our
applications such as our [AdoPiSoft](https://wwww.adopisoft.com) application and servers. Docker has made it so much easier to setup all these services with
a single configuration repository.

## System Requirements

- `docker`
- `make`

## Usage

```
git clone git@github.com:adonespitogo/docker-services.git ~/docker-services
cd ~/docker-services
cp .env.sample .env
```

Setup your environment variables by copying `.env.sample` to `.env` and modify the values in `.env` to suite your needs.

## MariaDB Service

To start `mariadb` server, type: `make start_mariadb`. To stop, use `make stop_mariadb`.

The default database access settings are:

```
host      = localhost
username  = root
password  = rootpass
port      = 3306
```

## Postgres Service

To start `postgres` server, type: `make start_postgres`. To stop, use `make stop_postgres`.

The default database access settings are:

```
host      = localhost
username  = postgres
password  = postgrespass
port      = 5432
```

