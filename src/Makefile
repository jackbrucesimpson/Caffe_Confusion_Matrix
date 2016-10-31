CC = g++
CFLAGS = -O3 -g -Wall -std=c++11 `pkg-config opencv --cflags`
LIBS = \
       `pkg-config opencv --libs` \
       -lboost_system \
       -lboost_timer \
       -lboost_filesystem \
       -lboost_program_options \
       -lcaffe \
       -lglog
SRCS = \
       Classifier.cpp \
       main.cpp
PROG = ../bin/confusion_matrix


$(PROG):$(SRCS)
	$(CC) $(CFLAGS) -o $(PROG) $(SRCS) $(LIBS)

clean:
	rm $(PROG)
