# Note: this makefile should be called by the makefile in the parent
# directory, which will pass it a number of variables defined there.
# To make the files here properly, try make util-bin or make util-debug
# from there.  Install *only* works at the top level; do make install-util
# and make install-uman.  make clean will work properly if called in
# this directory.

all: strfile unstr rot

strfile: strfile.o
	$(CC) $(CFLAGS) $(LDFLAGS) -o strfile strfile.o

unstr: unstr.o
	$(CC) $(CFLAGS) $(LDFLAGS) -o unstr unstr.o

randstr: randstr.o
	$(CC) $(CFLAGS) $(LDFLAGS) -o randstr randstr.o

rot: rot.o
	$(CC) $(CFLAGS) $(LDFLAGS) -o rot rot.o

clean:
	rm -f *.o unstr strfile randstr rot ansify
