# Simple PHP

## Introduccion

Este es un proyecto hola mundo simple en docker que muestra como construir, correr y borrar imagenes.  Incluye los siguientes archivos:

* Dockerfile
* src/index.php

La imagen se construye a partir de una imagen de php y apache.  

## Construir la imagen

```docker build -t hola-mundo .```

## Correr el contenedor

```docker run --name=hola-mundo -p8088:80 hola-mundo```

## Borrar el contenedor

Primero listar los contenedores que estan corriendo:

```docker ps -a```

Obtener el id del contenedor y correr

```docker rm -f <id-contenedor>```

## Borrar la imagen

Primero listar las imagenes con el comando:

```docker images```

Obtener el id de la imagen, y correr

```docker rmi -f <id-imagen>```
