# Docker Cheatsheet

## Información

```bash
docker images
docker ps
docker ps -a
docker system df
```

---

## Crear y ejecutar contenedores

```bash
docker run
docker exec
docker start
docker stop
docker restart
docker rm
```

---

## Imágenes

```bash
docker pull
docker build
docker image prune
docker image prune -a
```

---

## Volúmenes

Crear volumen:

```bash
docker volume create mydata
```

Listar volúmenes:

```bash
docker volume ls
```

Montar volumen:

```bash
docker run -v mydata:/data
```

---

## Redes

```bash
docker network ls
docker network prune
```

---

## Build cache

```bash
docker builder prune
```

---

## Limpieza

```bash
docker container prune
docker image prune
docker network prune
docker builder prune
docker system prune
docker system prune --volumes
```

---

## Flujo mental

```text
Imagen
↓
Contenedor
↓
Writable Layer
↓
Volumen
↓
Limpieza
```
