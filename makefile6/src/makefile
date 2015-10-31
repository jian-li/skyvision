IDIR =../include
CC=gcc
CFLAGS=-I$(IDIR)

ODIR=obj
LDIR =../lib

LIBS=-lm

_DEPS = $(wildcard IDIR/*.h)
DEPS = $(patsubst %,$(IDIR)/%,$(_DEPS))


_SRC = $(wildcard ./*.c) 
OBJ = $(patsubst %.c,$(ODIR)/%.o,$(_SRC))


$(ODIR)/%.o: %.c $(DEPS)
	$(CC) -c -o $@ $< $(CFLAGS)

hellomake: $(OBJ)
	gcc -o $@ $^ $(CFLAGS) $(LIBS)

.PHONY: clean

clean:
	rm -f $(ODIR)/*.o *~ core $(INCDIR)/*~ 
