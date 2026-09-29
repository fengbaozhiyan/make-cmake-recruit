CC = gcc
CFLAGS = -Wall -Wextra -Iinclude

calculator: main.o calculator.o logger.o
	# TODO: link object files into the calculator executable
	$(CC) $^ -o $@ 
main.o: src/main.c include/calculator.h include/logger.h
	# TODO: compile src/main.c
	$(CC) $(CFLAGS) -c $< -o $@ 
calculator.o: src/calculator.c include/calculator.h
	# TODO: compile src/calculator.c
	$(CC) $(CFLAGS) -c $< -o $@
logger.o: src/logger.c include/logger.h
	# TODO: compile src/logger.c
	$(CC) $(CFLAGS) -c $< -o $@
.PHONY: clean
clean:
	# TODO: remove calculator and all .o files
	rm -f calculator *.o
