# Makefile for echo_client and echo_server
CC = gcc
CFLAGS = -Wall -Wextra -g
LDFLAGS = -lpthread

# 디렉토리 및 파일
SRCDIR = .
TARGETS = client server

all: $(TARGETS)

client: $(SRCDIR)/echo_client.c $(SRCDIR)/csapp.c
	$(CC) $(CFLAGS) -o $@ $^ $(LDFLAGS)

server: $(SRCDIR)/echo_server.c $(SRCDIR)/csapp.c
	$(CC) $(CFLAGS) -o $@ $^ $(LDFLAGS)

clean:
	rm -f $(TARGETS)