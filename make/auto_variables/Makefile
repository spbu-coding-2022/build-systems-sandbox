TARGET = hello

CC = gcc
LD = gcc
CFLAGS = -c

.PHONY: all clean

all: $(TARGET)

main.o: main.c
	$(CC) $(CFLAGS) $< -o $@

hello.o: hello.c
	$(CC) $(CFLAGS) $< -o $@

$(TARGET): main.o hello.o
	$(LD) $^ -o $@

clean:
	rm -rf $(TARGET) *.o

