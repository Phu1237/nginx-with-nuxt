# Docker + Nginx + NuxtJS

## Create network

```bash
docker network create external
```

## Start and run

```bash
docker compose build
docker compose up -d
```

## Get logs

```bash
docker compose logs > logs.txt
```