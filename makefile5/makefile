CXXFLAGS = $(shell pkg-config --cflags opencv)
LIBS = $(shell pkg-config --libs opencv)

OBJS = $(patsubst %.cpp,%.o,$(wildcard *.cpp))

DisplayImage: $(OBJS)
	$(CXX) $< -o $@ $(LIBS) 

%.o: %.cpp
	@echo $(CXX)
	@echo $(OBJS)
	$(CXX) -c $< -o $@ $(CXXFLAGS)

clean:
	rm -f DisplayImage  *.o
