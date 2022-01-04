# lsh
LSH is a simple implementation of a shell in C, and it is the subject of a tutorial on this [website](https://brennan.io/2015/01/16/write-a-shell-in-c/). It demonstrates the basics of how a shell works.
# Running
Use `gcc -o lsh src/main.c` to compile, and then `./lsh` to run. If you would like to use the standard-library based implementation of `lsh_read_line()`, then you can do: `gcc -DLSH_USE_STD_GETLINE -o lsh src/main.c`.
# Contributing
### The original shell:
Is only: read, parse, fork, exec, and wait.
It had many limitations, including:
* Commands must be on a single line.
* Arguments must be separated by whitespace.
* No quoting arguments or escaping whitespace.
* No piping or redirection.
* Only builtins are: cd, help, exit.
### New features add by me:
