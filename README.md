# SIMPLE SHELL

## Table of Contents
1. [Description](#description-)
2. [Requirements](#requirements-)
3. [Installation and Compilation](#installation-and-compilation)
4. [Example of Use](#example-of-use-)
5. [Authors](#authors-%EF%B8%8F)

## Description

Simple-shell is a simple program of the line commands. This simple shell recreates basic and some more complex functionalities to result in our own Shell. This shell si developed in the programming language c. This shell takes the keyboard commands and delivers them to the system to be executed. some built-in commands implement: exit, env, help, cd.

## Requirements

Simple_shell is designed to run in the `Ubuntu 14.04 LTS` linux environment and to be compiled using the GNU compiler collection v. `gcc 4.8.4` with flags `-Wall, -Werror, -Wextra, -std=gnu89,and -pedantic`.

## Installation and Compilation

You need to clone [this repository](https://github.com/mehdielk11/simple_shell):
```
	git clone https://github.com/mehdielk11/simple_shell
```
and then you can compile with this command:
```
	gcc -Wall -Werror -Wextra -std=gnu89 -pedantic *.c -o hsh
```
after compilation you can excecute with this command:
```
	./hsh
```

## Example of Use

* Compile the program to create the `hsh` executable file (see instructions above).
* run the executable as follows `./hsh`
* Enter basic commands like: `ls`, you can add flags along with `ls` command such as `-l`, `-la`(`ls -l`, `ls -la`)
* press enter after entering the command
* to end the execution of the `simple_shell` program press `ctrl + d` or write the word `exit`

Your shell should work like this in interactive mode:
```
$ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
$
```
But also in non-interactive mode:
```
$ echo "/bin/ls" | ./hsh
hsh main.c shell.c test_ls_2
$
$ cat test_ls_2
/bin/ls
/bin/ls
$
$ cat test_ls_2 | ./hsh
hsh main.c shell.c test_ls_2
hsh main.c shell.c test_ls_2
$
```
## Authors

Mehdi ELKHEMLICHI (https://github.com/mehdielk11)
