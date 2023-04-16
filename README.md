# Docker + Nginx + NuxtJS

## Create network

```bash
docker network create external
```

## How to use

1. Duplicate the .env.example file and name it .env
2. Put the source code in the src/client directory and src/server
3. Build and run the Docker
4. Client will serve at http://localhost/ and serve at http://localhost/api/

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