
default: exam

CC     = gcc
CFLAGS = -Wall -Wextra -O2 -g -Wmissing-declarations -Wmissing-prototypes -Wimplicit-function-declaration -Wunused -Wuninitialized -Wvla -Wformat -Wformat-security -Wmain -Wsequence-point -Wshadow -Wbad-function-cast -Wcomments -Wdeclaration-after-statement -Waddress -Wpointer-sign -Wempty-body -Wnested-externs -Wold-style-declaration -Wold-style-definition -Wmissing-field-initializers -Wmaybe-uninitialized -Wno-return-local-addr -Wreturn-type -Wsequence-point -Wundef -Wunknown-pragmas -Wunused-label

exam: exam.o projmgmt.o
	$(CC) -o exam exam.o projmgmt.o

exam.o: exam.c projmgmt.h
	$(CC) $(CFLAGS) -c exam.c

projmgmt.o: projmgmt.c projmgmt.h
	$(CC) $(CFLAGS) -c projmgmt.c

clean:
	rm -fv exam *.o
