# UNIX Tutorial for Beginners

## UNIX Introduction

### Types of UNIX

- Sun Solaris
- GNU/Linux
- MacOS X

### The UNIX operating system

3 parts:  kernel, shell, programs.

1. The kernel

   - allocates time and memory to programs

   - handles the filestore and communications in response to system calls

   - an illustration of kernel and shell working together:

     - A user types in `rm myfile`
     - The shell searches filestore for the file containing `rm`
     - The shell requests kernel through system calls
     - The kernel executes the program `rm`
     - When `rm` has finished running, the shell returns `%`  to the user

     <!-- % is an UNIX prompt indicating that it is waiting for further commands.-->

2. The shell

   - an interface between the user and the kernel
   - a program started right after you log in
   - a command line interpreter (CLI)

### Files and processes

Everything in UNIX is either a file or a process.

1. process
   - an executing program identified by a unique PID (process identifier)
2. file
   - a collection of data
   - created by users using text editors, running compilers, etc.
   - Examples:
     - a document
     - the text of a program in some high-level language
     - instructions comprehensible directly to the machine but not human, e.g. an executable or binary file
     - a directory (top level directory is called ' \ ')

## Tutorial 1

`% ls `  see  what is in the directory (partly)

`% ls -a`  also see the files beginning with a dot (.) (hidden files containing  program configuration information)

`% mkdir` make directory

(.) a dot means current directory

(..) 2 dots means the parent of the current directory

(~) tilde means home directory

`% pwd` print working directory

## Tutorial 2

`% cp file1 file2`  makes a copy of file1 in the current working directory and calls it file2. (file1 may be a path, i.e. a file from another directory)

`% mv file1 file2`  moves file1 to file2; also used to rename a file (in the same directory)

`% rm file1` removes file1

`% rmdir dir1` removes dir1 (directory)

`% clear` clear screen

`% cat file1.xx` (concatenate) show the content of the file on the screen

`% less file1.xx`  show one page of the file on the screen at a time, press the `space-bar` to see another page and type `q`  to quit reading. (used for long files in replace of `cat`)

`% head file1.xx` show the first 10 lines (default, can change using flag e.g. -5) of file1

`% tail file1.xx` show the last 10 lines of file1

`% grep keyword file.xx`  search the file for keyword. If it is not a single word, use ''.

​	`	-i` ignores upper/lower case distinctions; `-v` displays those lines that do NOT match;

​	`-n ` precedes each matching line with the line number; `-c`  print only the total count of matched lines.

`% wc keyword file.xx`  word count.

​	`-w`  do a word count; `-l`  find how many lines in the file.