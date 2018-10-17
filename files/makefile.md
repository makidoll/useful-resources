# Examples of a Makefile

https://www.gnu.org/software/make/manual/html_node/Implicit-Variables.html
https://www.gnu.org/software/make/manual/html_node/Using-Implicit.html#Using-Implicit
https://www.gnu.org/software/make/manual/html_node/Catalogue-of-Rules.html#Catalogue-of-Rules

```makefile
CC = gcc
CFLAGS = -Wall
LDFLAGS = -lm
OUT = Test

SRCS = $(wildcard src/*.c)
OBJS = $(SRCS:src/%.c=src/%.o)

all: $(OBJS)
	$(CC) $(OBJS) $(CFLAGS) $(LDFLAGS) -o $(OUT)

.PHONY: clean
clean: 
	rm -rf src/*.o
```
