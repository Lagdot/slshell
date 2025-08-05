very simple shell in C and assembly

# Building
you'll need gcc and the gnu binutils or any c compiler, assembler and linker
these instructions are for gcc and gnu binutils though
I am NOT making a Makefile

```
git clone https://github.com/Lagdot/slshell
cd slshell
gcc -c shell.c --no-stack-protector
as sys.S
ld -o shell shell.o a.out --entry main -z noexecstack
```

and then just run it `./shell`
