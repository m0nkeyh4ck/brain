
#trtamiento_de_la_tty

```bash
1) script /dev/null -c bash
2) ^Z
3) stty raw -echo
4) fg
5) reset
6) xterm
7) export TERM=xterm
8) export SHELL=bash
9) stty -a
10) stty size
11) stty rows 27 columns 127
```

#con_python

```bash
1) python -c 'import pty;pty.spawn("/bin/bash")'
2) ^Z
3) stty raw -echo
4) fg
5) reset
6) xterm
7) export TERM=xterm
8) export SHELL=bash
9) stty -a
10) stty rows 27 columns 127
```