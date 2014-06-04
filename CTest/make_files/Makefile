DEFAULT	= main
OBJECTS	= $(DEFAULT).o common.o


CC	= gcc

all: $(DEFAULT)

%.o : %.c
	$(CC) $(CFLAGS) -c $<

#%.o : %.cu
#	$(CC) $(CFLAGS) -c $<

$(DEFAULT) : $(OBJECTS)
	$(CC) $(CFLAGS) -o $@ $^
	-@rm -f *.o 2>&1 > /dev/null


.PHONY: clean all

clean :
	-@rm -f *.o $(DEFAULT) 2>&1 > /dev/null
