#target:prerequest
#<#tab>:command
#declaration of variable 
file=test.c

display:
	@echo "hello"

build:
	gcc $(file) -o test.o

all: display
	gcc $(file) -o test

clean:
	@rm *.o
	@echo "'date 'done" > log.txt

