# Cosas de Docker

> Aprendiendo cosas importantes en Docker.

## Summary

* [Ejemplos](#ejemplo)
	* [Subida de archivo](#subida-de-archivos)
	* [Content Type](#content-type)
	* [Magic Number](#magic-number)

## Php

### Ejemplos

`docker hub` en esta página puedo buscar los contenedores a descargar


```bash
1) docker pull mysql     //descarga la ultima versión de mysql
2) docker pull mysql:12   //descarga la versión 12 de mysql
```

```bash
1) docker star monguito     //corre el contenedor
2) docker stop monguito  //detiene el contenedor
3) docker rm monguito    //eliminamos el contenedor
4) docker ps -a   //vemos los contenedores ocultos
5) docker logs monguito   // muestra los logs solo hasta donde ejecutaste este comando
6) docker logs --follow monguito    //muestra los logs y se queda escuchando
```


```bash
1) docker create "nombre de la imagen"     //crea un contenedor con la imagen que se le pase
2) docker create --name monguito "nombre de la imagen"  //crea el contenedor con la imagen pero nosotros le ponemos nombre
3) docker create -8080:80 -name monguito "nombre de la imagen"  //el 80 del docker es el 8080 del la maquina anfitrion
4) docker run mongo   //descarga la imgen , desplega el contenedor y queda mostrando los logs
5) docker run -d mongo  // descarga, desplega, pero no se queda en los logs, solo te devuelve la terminal normal
```

port maping, vamos a mapear puertos, es decir, que un puerto especifico del contenedor se sincronice con un puerto nestro
