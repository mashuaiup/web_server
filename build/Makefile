CXX = g++
CFLAGS = -std=c++14 -O2 -Wall -g 

TARGET = server
OBJS = ../code/log/*.cpp ../code/pool/*.cpp ../code/timer/*.cpp \
       ../code/http/*.cpp ../code/server/*.cpp \
       ../code/buffer/*.cpp ../code/main.cpp

LDLIBS = -L/root/protocol_stack/build
CFLAGS += -I/root/protocol_stack
CFLAGS += -I/root/protocol_stack/std

all: $(OBJS)
	$(CXX) $(CFLAGS) $(OBJS) -o ../bin/$(TARGET) $(LDLIBS) -ldpdk -lprotostack -pthread -lmysqlclient
clean:
	rm -rf ../bin/$(TARGET)




