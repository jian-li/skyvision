CXXFLAGS = $(shell pkg-config --cflags opencv)
LIBS = $(shell pkg-config --libs opencv)
CXX = g++

OBJS = $(patsubst %.cpp,%.o,$(wildcard *.cpp))

DisplayImage: $(OBJS)
	$(CXX) $< -o $@ -L$(LIBS) 

%.o: %.cpp
	$(CXX) -c $< -o $@ -I$(CXXFLAGS)

clean:
	rm -f DisplayImage  *.o
