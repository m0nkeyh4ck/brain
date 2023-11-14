

```bash
1) find / -prem -4000 2>/dev/null   //busca binarios SUID
2) find / -user "jesus" 2>/dev/null 
3) find / -type f -user jesus 2>/dev/null //busca archivos que le pertenezcan a jesus
4) find / -type f -group admin 2>/dev/null //busca archivos que le pertenezcan al grupo admin
```