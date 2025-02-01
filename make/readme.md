In this i want to talk about process of compilation :
the process of compilation involved four steps :
preprocessing 
compilation 
assembler 
linker 

i will explain step by steps :
preprocessing 
:it will eliminate  the comment  and replace the include file by it's contenu .
use the fllowing  commands :
cpp main.c -o main.i (for c code )(main.ii for c++ code )

compilation :
it will generate assebly code :file (main.s )
gcc -S main.i 

assembler :
as main.s -o main.o (the first step object file ;format ELF  :executable and linkable format )


linker :it will generate executable file (machine code that can by understood by cpu )
 gcc main.i  -o main 



For makefile :
we use it when we have a big project where several file  need to be compiled in specific  order with specific rules .

and to compile this file use tool (make) or (make -f name-makefile
for example the name of makefile is build 
so execute this command :
make -f build ::


example about makefile contenu :
all:
#	gcc main.c calcul.c  -o cal 
