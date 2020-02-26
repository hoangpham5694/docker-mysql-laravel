# Sales POS Docker Setting

## Prequisites

- Docker. Visit [installation guide](https://www.docker.com/community-edition)
- Docker Compose. Visit [installation guide](https://docs.docker.com/compose/install/)


## Preparation

- Make sure cloning 2 repositories into the same directory

```
... health_portal/
... health_portal-docker/
```


## Builder Docker Images Steps:

### 1. Create .env file by copying .env.example

```
$ cp .env.example .env
```

### 2.  Build docker containers

```
$ docker-compose build
```

### 3. Run docker containers

```
$ docker-compose up -d
```

> -d: detach mode

### 4. Access to web container as "health-portal" user

```
$ docker-compose exec --user=health-portal web bash
```
