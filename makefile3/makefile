CXXFLAGS = $(shell pkg-config --cflags opencv)
LIBS = $(shell pkg-config --libs opencv)
CXX = g++

DisplayImage: DisplayImage.o
	$(CXX) $< -o $@ -Wall -L$(LIBS) 

DisplayImage.o: DisplayImage.cpp 
	$(CXX) -c $< -o $@ -I$(CXXFLAGS)

clean:
	rm -f  DisplayImage *.o
