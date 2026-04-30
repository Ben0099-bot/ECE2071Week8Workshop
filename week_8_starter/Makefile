all: outputs/program

outputs/program: outputs/main.o outputs/stats.o
	gcc outputs/main.o outputs/stats.o -o outputs/program

outputs/main.o: src/main.c
	gcc -c src/main.c -o outputs/main.o

outputs/stats.o: src/stats.c
	gcc -c src/stats.c -o outputs/stats.o
