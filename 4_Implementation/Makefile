ifdef OS
	RM=del /q
	FixPath=$(subst /,\,$1)
	EXEC=exe
else
	ifeq ($(shell uname),Linux)
	RM=rm .rf
	FixPath=$1
	EXEC=out
	endif
endif


build: main.c features.c features.h
	gcc main.c features.c features.h  -o g.out
run:
	./g.out
clean:
	rm *.out