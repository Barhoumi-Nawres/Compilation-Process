CC = gcc
CFLAGS = -Wall -c

all: cal

main.o: main.c cal.h
	$(CC) $(CFLAGS) main.c -o main.o

cal.o: cal.c cal.h
	$(CC) $(CFLAGS) cal.c -o cal.o

cal: main.o cal.o
	$(CC) main.o cal.o -o cal

clean:
	rm -f *.o cal

