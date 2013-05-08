CC = gcc
CFLAGS = -g

a.out: main.o prog1.o slp.o util.o
	$(CC) $(CFLAGS) main.o prog1.o slp.o util.o

main.o: main.c slp.h util.h
	$(CC) $(CFLAGS) -c main.c

prog1.o: prog1.c slp.h util.h
	$(CC) $(CFLAGS) -c prog1.c

slp.o: slp.c slp.h util.h
	$(CC) $(CFLAGS) -c slp.c

util.o: util.c util.h
	$(CC) $(CFLAGS) -c util.c

clean: 
	rm -f a.out util.o prog1.o slp.o main.o
