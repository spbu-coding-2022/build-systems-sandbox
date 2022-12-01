TARGET = hello

CC = gcc
LD = gcc
CFLAGS = -c

.PHONY: all clean

all: $(TARGET)

main.o: main.c
	$(CC) $(CFLAGS) main.c -o main.o

hello.o: hello.c
	$(CC) $(CFLAGS) hello.c -o hello.o

$(TARGET): main.o hello.o
	$(LD) main.o hello.o -o $(TARGET)

clean:
	rm -rf $(TARGET) *.o

