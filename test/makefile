Target = test
Objects = test.o

CC = gcc
Compile = $(CC)
Link = $(CC) -lstdc++

LIB = -Wall -lz -lrt -ldl -lpthread \
	-L./ -lx264 

main :  $(Objects)    
	$(Link) $(Objects) $(LIB) -o $(Target)


.cpp.o :
	$(Compile) -c -o $@ $< $(INCLUDE)
.c.o :
	$(Compile) -c -o $@ $< $(INCLUDE)	
clean:
	rm *.o

#	rm $(Target)

