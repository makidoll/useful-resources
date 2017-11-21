# Examples of a Makefile

```
CC = gcc
OBJS = main.c
FLAGS = -Wall
LNK = -lncurses
OUT = bin/game

all: $(OBJS)
	$(CC) $(FLAGS) $(LNK) $(OBJS) -o $(OUT)

clear: 
	rm -rf /
```