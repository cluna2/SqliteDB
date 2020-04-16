CC = gcc
CFLAGS = -O0 -g3 -Wall
CFLAGS += -std=gnu99 -g 
EXECS = sqlite_clone
HEADERS = simple_compiler.h
SOURCES = sqlite_main.c simple_compiler.c 

.PHONY: all clean

all: $(EXECS)

sqlite_clone: $(HEADERS) $(SOURCES)
	$(CC) $(CFLAGS) $(SOURCES) -o sqlite_clone

clean:
	rm -rf $(EXECS)

format: *.c
	clang-format -style=Google -i *.c