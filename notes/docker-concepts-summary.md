Docker Concepts Summary

¿Qué es Docker?

Docker permite ejecutar aplicaciones dentro de contenedores aislados y reproducibles.

La idea principal es:

Imagen → Contenedor → Datos → Limpieza

⸻

Imagen

Una imagen es una plantilla inmutable.

Ejemplos:

* alpine
* ubuntu
* hello-world

Pensamiento:

Imagen = receta

⸻

Contenedor

Un contenedor es una imagen ejecutándose.

Comandos principales:

* docker run
* docker stop
* docker start
* docker restart
* docker rm

Pensamiento:

Contenedor = aplicación en ejecución

⸻

Ciclo de vida

Estados:

* Crear
* Ejecutar
* Detener
* Reiniciar
* Eliminar

⸻

Writable Layer

La capa writable es temporal.

Los cambios pertenecen al contenedor.

Si el contenedor se elimina, los datos desaparecen.

⸻

Volúmenes

Los volúmenes almacenan datos persistentes.

Comandos:

* docker volume create
* docker volume ls

Idea importante:

Contenedor eliminado ≠ volumen eliminado

⸻

Limpieza

Comandos:

* docker system df
* docker container prune
* docker image prune
* docker network prune
* docker builder prune
* docker system prune

⸻

Mapa Mental

Imagen
↓
Contenedor
↓
Writable Layer
↓
Volumen
↓
Limpieza

⸻

Filosofía

No memorizar comandos.

Comprender:

Imagen → Contenedor → Datos → Mantenimiento