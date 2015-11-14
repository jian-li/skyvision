
CFLAGS = $(shell pkg-config --cflags opencv)

LIBS = $(shell pkg-config --libs opencv)

DisplayImage: DisplayImage.o
	g++ -o DisplayImage DisplayImage.cpp -I$(CFLAGS) -L$(LIBS)

clean:
	rm -f *.o DisplayImage
