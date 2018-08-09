CC = g++
PROG = teste
CPPFLAGS = -Iinclude -Wall -pedantic -std=c++11
BUILD = ./build
SRC = ./src
BIN = ./bin

OBJS = $(BUILD)/circulo.o $(BUILD)/calculadorArea.o $(BUILD)/retangulo.o $(BUILD)/triangulo.o $(BUILD)/main.o 

all: $(OBJS)
	$(CC) $(CPPFLAGS) -o $(BIN)/$(PROG) $(OBJS)

$(BUILD)/circulo.o:
	$(CC) $(CPPFLAGS) -c $(SRC)/circulo.cpp -o $(BUILD)/circulo.o

$(BUILD)/calculadorArea.o:
	$(CC) $(CPPFLAGS) -c $(SRC)/calculadorArea.cpp -o $(BUILD)/calculadorArea.o

$(BUILD)/retangulo.o:
	$(CC) $(CPPFLAGS) -c $(SRC)/retangulo.cpp -o $(BUILD)/retangulo.o

$(BUILD)/triangulo.o:
	$(CC) $(CPPFLAGS) -c $(SRC)/triangulo.cpp -o $(BUILD)/triangulo.o

$(BUILD)/main.o:
	$(CC) $(CPPFLAGS) -c $(SRC)/main.cpp -o $(BUILD)/main.o