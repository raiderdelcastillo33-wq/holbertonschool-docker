# Docker Concepts Summary

## **Idea principal**

Docker permite ejecutar aplicaciones dentro de contenedores aislados, reproducibles y fáciles de compartir.

Modelo mental:

```
Imagen → Contenedor → Datos → Limpieza
```

## **Imagen**

Una imagen es una plantilla inmutable.

Ejemplos:

- alpine
- ubuntu
- hello-world

## **Contenedor**

Un contenedor es una imagen ejecutándose.

Tiene:

- proceso principal
- filesystem temporal
- aislamiento

## **Writable Layer**

La writable layer guarda cambios temporales del contenedor.

Si el contenedor se elimina, esta capa desaparece.

## **Volúmenes**

Los volúmenes permiten persistir datos fuera del contenedor.

Idea clave:

```
Contenedor eliminado ≠ volumen eliminado
```

## **Limpieza**

Docker acumula contenedores detenidos, imágenes, redes y caché.

Comandos clave:

```
docker system df
docker container prune
docker image prune
docker network prune
docker builder prune
docker system prune
```
