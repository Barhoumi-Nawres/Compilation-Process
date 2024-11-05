#target:prerequest
#<#tab>:command
#declaration of variable 
file=test.c

build:
	gcc $(file) -o test.o

all: display
	gcc $(file) -o test

clean:
	@rm *.o
	@echo "`date` done" > log.txt

define display
	@echo "makefile-function"
endef

target1:
	$(call display)
	@echo
###############
LIST= 1 2 3 4 5 6 7 8 9 10 11 12 13  14 15
loop1:
	@for i in $(LIST); do \
		echo $$i; \
	done
##############

