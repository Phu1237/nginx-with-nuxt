# Docker + Nginx + NuxtJS

## Create network

```bash
docker network create external
```

## Start and run

### Build the Docker image

```bash
docker compose build
```

### Run the Docker container

- Using Proxy server (OpenLiteSpeed)

```bash
docker compose -f docker-compose.yml -f docker-compose.proxy.yml up -d
```

- Using PHP-FPM

```
docker compose -f docker-compose.yml -f docker-compose.php-fpm.yml up -d
```

## Get logs

```bash
docker compose logs > logs.txt
```