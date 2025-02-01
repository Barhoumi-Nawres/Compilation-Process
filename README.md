# Compilation-Process
this repository explain how the compilation process work  and how to use the Makefile :
# Compiler:
a Compiler is a software program that translate high-level programming language code into machine code that can be understood by a microcontroller processor .

## Table of contents :
- [Process of compilation ](#Process-of-compilation)
- [Makefile](#Makefile)
## Process of compilation :
Compilation process in C involves four steps: pre-processing, compiling, assembling, and linking.
- [Pre-processing](#Pre-processing):
this is the first step that replace  the content of include library and rmove all comments .
use the fllowing command:

```bash
cpp main.c -o main.i
```
 (.i for c code and .ii for c++ code )
  
- [Compiling](#Compiling):
  the command :
```bash
  gcc -S main.i
```


  (it will generate (.s file=assembly code  )
  
- [Assembler](#Assembler):
```bash
 as main.s -o main.o
```

(it will generate object file )
  
- [Linking](#Linking):
 there are two types of linker static and dynamic :
use the fllowing command:
```bash
gcc main.o -o main
```
(it will generate  executable code (machine code that can be understood by cpu )(ELF :Executable and linkable format )


## Makefile:  
the makefile is very useful for managing a large projects ,where several files must be compiled in a specific order with a specific  rules .
