
este comando nos ayuda a filtrar la información

## grep

```bash
1) grep -oP '\d{1,5}/open'  //te filtra los dijitos del 1 al 5 de longitu, y que alado tenga la palabra open
2) grep -oP '\w{1,10}.*'  // fitra por una palabra que termine máximo 10 de linguitud y el .* es todo lo que sigue  
3) grep -oP '\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}'  //esto ayuda a filtrar la ip
4) grep -A 1  //una line abajo
5) grep -B 1  //una line arriba
6) grep -C 1  //una line abajo y arriba
7) grep -oP "^algo$"  //busca algo que empiece y termine con la palabra algo
8) grep -r -i "fasdfhsd" /    //busca de forma recurciba lo que le digas desde la raiz
```

## sed

```bash
1) sed '/^\s*$/d'  //quita estacios o filas sin contenido
2) sed 's/^ *//'   //quita los espacio del comienzo 
```

## xargs

```bash
1) xargs // sirve para paralelisar la salida de un comando
```

## cut

```bash
1) cut -d '/' -f 1   //primer argumento y el delimitador es /
2) cut -d '/' -f 1-3
3) cut -d '/' -f 1-5
```

## awk

```bash
1) awk '{print $1}' FS='/'  //filtra el primer argumento y el delimitador es el /
```

## tr

```bash
1) tr ' ' ','  //reemplaza los espacios por coma
2) tr -d '\n'  //elimina los saltos de linea
```