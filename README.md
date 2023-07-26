Simple Unix Shell

**Table of Contents**

Description
Environment
File Structure
Requirements
Installation
Usage
Feature
Workflow
Example of Use
Bugs
Staff
License

**Description** 
The simple_shell is a script that takes text file that contains a sequence of commands for a UNIX-based operating system. It is called a shell script because it combines a sequence of commands, that would otherwise have to be typed into the keyboard one at a time, into a single script. It is written in C.

*List of allowed functions and system calls in this simple shell are:*
access (man 2 access)
chdir (man 2 chdir) 
execve (man 2 execve)
exit (man 3 exit) 
fork (man 2 fork)
free (man 3 free) 
getline (man 3 getline) 
isatty (man 3 isatty) 
malloc (man 3 malloc) 
perror (man 3 perror) 
signal (man 2 signal) 
strtok (man 3 strtok)
wait (man 2 wait) 
write (man 2 write)

**Environment** <br>
Suite CRM OS: Ubuntu 22.04 LTS terminal C Low level programming language Language: C Compiler: gcc 11.3.0 
Suite CRM Editor: VIM 8.2.3995
git distributed version control system Control version: Git 
Github 
Style guidelines: Betty style 

**File Structure**<br>
Below are files with general information about the program:

AUTHORS - List of individuals that contributed to the success of this program and its repo.
man_simple_shell - Manual page for the simple_shell
shell.h - Header file with fuction prototypes

- hsh - the executable to run the shell
- builtin.c - Handles inbuilt commands
- strtoken.c - tokenizes input commands
- charFun.c - manipute input characters
- exeFile.c - Read Command from file
- execute.c - Handle builtin commands
- pathFinder.c - search in path for executable command
- getLine.c - Read the stdin by user 
- hist.c - Fill file by user input
- mem_manager.c - Handles memory allocation
- moreBul.c - history of user input
- moreCharfun.c - compare how much different
- moreFun.c - copy of characters
- output.c - handles stdout and error commands
- parser.c - handles user input to parse
- printer.c - prints unsigned int putchar
- prompter.c - display shell prompt
- shell.c - handles arg count and arg value
- shell.h - handles prototypes of all the functions used

**Installation**<br>
- Clone this repository: git clone "https://github.com/habeebhassan/Simple-Shell"
- Change directories into the repository: cd simple_shell
- Compile: gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
- Run the shell in interactive mode: ./hsh
- Or run the shell in non-interactive mode: example echo "Hello world!" | ./hsh

**Features**<br>
- Implement the use of builtins commands
- shell halts using Crtl+D or EOF
- handles command line arguments

**Examples of Use Case**<br>
- In interactive mode

 $ ./hsh
($) /bin/ls
hsh main.c shell.c
($)
($) exit
/$

- In non-interactive mode

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
/$

**Bugs**<br>
Bugs are not found

**Staff**<br>
<a href="linkedin.com/n/habeebhassan08">Habeeb hassan | Linkedin</a>

**License**<br>
The project is written under MIT. Contributors are highly welcome
