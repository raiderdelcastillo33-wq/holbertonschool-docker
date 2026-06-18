# Docker Cheatsheet

## Información

```bash
docker images
docker ps
docker ps -a
docker system df
```

## **Crear y ejecutar contenedores**

```
docker run
docker exec
docker start
docker stop
docker restart
docker rm
```

## **Imágenes**

```
docker pull
docker build
docker image prune
docker image prune -a
```

## **Volúmenes**

```
docker volume create mydata
docker volume ls
docker run -v mydata:/data
```

## **Redes**

```
docker network ls
docker network prune
```

## **Build cache**

```
docker builder prune
```

## **Limpieza**

```
docker container prune
docker image prune
docker network prune
docker builder prune
docker system prune
docker system prune --volumes
```

## **Flujo mental**

```
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
