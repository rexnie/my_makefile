objects = main.o print1.o print2.o
CC = gcc

empty:=
space:= $(empty) $(empty)

all_c=$(wildcard *.c)
all_o=$(patsubst %.c, %.o, $(all_c))

main.bin : $(objects)
	@$(CC) -o $@ $^
	@echo $(MAKELEVEL)
	@echo $(all_c)
	@echo $(all_o)

main.o : print1.h print2.h

print1.o : print1.h

print2.o : print2.h

.PHONY : clean
clean :
	@-rm -r main.bin $(objects)
