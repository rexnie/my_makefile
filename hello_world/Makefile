main.bin : main.o print1.o print2.o 
	gcc -o main.bin main.o print1.o print2.o 

main.o : main.c print1.h print2.h
	gcc -o main.o -c main.c

print1.o : print1.c print1.h
	gcc -o print1.o -c print1.c

print2.o : print2.c print2.h
	gcc -o print2.o -c print2.c

clean :
	rm -r main.bin main.o print1.o print2.o  
