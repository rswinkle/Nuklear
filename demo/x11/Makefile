# Install
BIN = demo

# Flags
CFLAGS += -g -std=c89 -Wall -Wextra -pedantic -Wno-unused-function

SRC = main.c
OBJ = $(SRC:.c=.o)

$(BIN):
	@mkdir -p bin
	rm -f bin/$(BIN) $(OBJS)
	$(CC) $(SRC) $(CFLAGS) -D_POSIX_C_SOURCE=200809L -o bin/$(BIN) -lX11 -lm
