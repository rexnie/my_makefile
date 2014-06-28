objects = main.o print1.o print2.o
CC = gcc

main.bin : $(objects)
	$(CC) -o $@ $^

main.o : print1.h print2.h

print1.o : print1.h

print2.o : print2.h

.PHONY : clean
clean :
	-rm -r main.bin $(objects)
