# Makefile

# Compiler
CC = gcc

# Compiler flags
CFLAGS = -Wall -g

# Source files
SRCS = main.c string_operations.c

# Object files
OBJS = $(SRCS:.c=.o)

# Executable name
EXEC = my_program

# Default target
all: $(EXEC)

# Rule to build executable
$(EXEC): $(OBJS)
	$(CC) $(CFLAGS) -o $@ $^

# Rule to build object files
%.o: %.c
	$(CC) $(CFLAGS) -c -o $@ $<

# Clean target
clean:
	rm -f $(OBJS) $(EXEC)
