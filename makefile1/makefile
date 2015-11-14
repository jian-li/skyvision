DisplayImage: DisplayImage.o
	g++ -o DisplayImage DisplayImage.o -L/usr/local/lib -lopencv_core -lopencv_highgui -lopencv_imgcodecs 

DisplayImage.o: DisplayImage.cpp
	g++ -c DisplayImage.cpp -o DisplayImage.o -I/usr/local/include/opencv -I/usr/local/include

clean:
	rm -f DisplayImage *.o
