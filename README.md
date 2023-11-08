markdown
Copy code
# Simple Shell by Scofield Idehen

This is my self-owned simple shell implemented in C language.

## About

A shell is a user interface used to access the services of a computer. It can be a command-line interface – the one I've built – or a graphical user interface, like regular software such as Windows Office.

## Compilation

This simple shell can be compiled using the following command:

```shell
gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh
Output
This program produces the same output as the standard shell (sh) and the same error output. The only difference is that when it prints an error, the program's name is equivalent to argv[0].

Example of an error with sh:

shell
Copy code
$ echo "qwerty" | /bin/sh
/bin/sh: 1: qwerty: not found
$ echo "qwerty" | /bin/../bin/sh
/bin/../bin/sh: 1: qwerty: not found
Error with my program:

shell
Copy code
$ echo "qwerty" | ./hsh
./hsh: 1: qwerty: not found
$ echo "qwerty" | ./././hsh
./././hsh: 1: qwerty: not found
Testing
My shell works like this in interactive mode:

shell
Copy code
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
If a command is not found, it produces an error like this:

shell
Copy code
$ Ethio
./hsh: No such file or directory
Author
Scofield Idehen - GitHub Profile
