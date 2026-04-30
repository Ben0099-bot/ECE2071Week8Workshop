all: outputs/program

outputs/program: outputs/main.o outputs/stats.o
	gcc outputs/main.o outputs/stats.o -o outputs/program

outputs/main.o: src/main.c src/stats.h
	gcc -c src/main.c -o outputs/main.o

outputs/stats.o: src/stats.c src/stats.h
	gcc -c src/stats.c -o outputs/stats.o

test: tests/test_stats.c src/stats.h outputs/stats.o
	gcc outputs/stats.o tests/test_stats.c -o outputs/tests
