
#processs of compilation 
1- processing ->processor (delete all the comments and see the include .h file
we can use this command gcc -E file-name 
 -the objetif of the step preprocessing is delete include line  and remplece them by their file contain .
2-Assemblling -> .s file  using this command gcc -S file-name ,in the output filee  you will the assembly language 
 
3-Compilation ->take input in assembly language and convert it inti binary form or object code .
we can use the linux command gcc -c file-name  like this gcc -o (o:output)file -name  file-name-output.o 
After thsi commendd we will find the execution file .o
THE COMMAND is :gcc -c file-name.c 

4-Linker->the input is object code ,processed by Linker .linker will copy the definition of functions  and add it into the binary file /excutable file 
the Command is:gcc -o binary-name objectfile 
Now i will expalin compilation process more  in detail why we need in frensh :


dans le systsème linux nous avons trois partie /usespace/kernel space /hw (hardware )
la plus important partie dans hw (c'est le CPU contient les registres et des autres choses  )
-notre objectif c'est d'avoir des instructions travaille sur ce processeur 
les choces qu'il faut connaitre :
1/Architecture du processeur pour savoir comment on créer les instructions 
 (ARM,X86 ,MIPS ....etc )
chaque architecture a ISA (instruction set Architecture )
An Instruction Set Architecture (ISA) is part of the abstract model of a computer. It defines how software controls the processor. 



