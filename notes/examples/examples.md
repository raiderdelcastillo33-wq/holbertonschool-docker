# Docker Examples

## **Contenedor interactivo Alpine**

```
docker run -it --name lifecycle-demo alpine sh
```

## **Crear archivo temporal dentro de un contenedor**

```
echo "persistent?" > /tmp/testfile.txt
ls /tmp
```

## **Montar un volumen**

```
docker volume create mydata
docker run -it --name volume-demo -v mydata:/data alpine sh
```

## **Escribir dentro del volumen**

```
echo "saved across containers" > /data/example.txt
ls /data
```

## **Limpiar contenedores detenidos**

```
docker container prune
```

## **Ver uso de disco Docker**

```
docker system df
```
