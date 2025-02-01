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
This is the first step, where the compiler:

  -Replaces the content of included libraries (#include).
  -Removes all comments.
Use the following command:

```bash
cpp main.c -o main.i
```
The generated file has the .i extension for C and .ii for C++.
  
- [Compiling](#Compiling):
  The following command compiles the preprocessed file into assembly code:
  the command :
```bash
  gcc -S main.i
```

📌 Output: A .s file containing assembly code.
  
- [Assembling](#Assembling):
  The assembler converts the assembly code into an object file:
```bash
 as main.s -o main.o
```

(it will generate object file )
  
- [Linking](#Linking):
The linker combines object files into an executable file. There are two types of linkers: static and dynamic.
use the fllowing command:
```bash
gcc main.o -o main
```
📌 Output:

    An executable file containing machine code that the CPU can understand.
    The executable follows the ELF (Executable and Linkable Format).



## Makefile:  
the makefile is very useful for managing a large projects ,where several files must be compiled in a specific order with a specific  rules .
it's automation  of the compilation process :
Use the tool make  to execute the makefile (if the  name of makefile !=makefile so Use make -f name-of-makefile )

