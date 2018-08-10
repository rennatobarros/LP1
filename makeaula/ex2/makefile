CC = g++
PROG1 =$(BIN)/circulo
PROG2 =$(BIN)/triangulo
PROG3 =$(BIN)/retangulo

SRC = ./src
BIN = ./bin
INC = ./include
BUILD = ./build
CPPFLAGS = -Wall -pedantic -std=c++11 -I$(INC)

all: $(PROG1) $(PROG2) $(PROG3)

	$(PROG1): $(BUILD)/circulo.o $(BUILD)/circuloMain.o
		$(CC) $(CPPFLAGS) -o $(PROG1) $(BUILD)/circulo.o $(BUILD)/circuloMain.o

	$(PROG2): $(BUILD)/triangulo.o $(BUILD)/trianguloMain.o
		$(CC) $(CPPFLAGS) -o $(PROG2) $(BUILD)/triangulo.o $(BUILD)/trianguloMain.o

	$(PROG3): $(BUILD)/retangulo.o $(BUILD)/retanguloMain.o
		$(CC) $(CPPFLAGS) -o $(PROG3) $(BUILD)/retangulo.o $(BUILD)/retanguloMain.o

	$(BUILD)/circulo.o: $(SRC)/circulo.cpp $(INC)/circulo.h
		$(CC) $(CPPFLAGS) -c $(SRC)/circulo.cpp -o $(BUILD)/circulo.o

	$(BUILD)/triangulo.o: $(SRC)/triangulo.cpp $(INC)/triangulo.h
		$(CC) $(CPPFLAGS) -c $(SRC)/triangulo.cpp -o $(BUILD)/triangulo.o

	$(BUILD)/retangulo.o: $(SRC)/retangulo.cpp $(INC)/retangulo.h
		$(CC) $(CPPFLAGS) -c $(SRC)/retangulo.cpp -o $(BUILD)/retangulo.o

	$(BUILD)/calculadorArea.o: $(SRC)/calculadorArea.cpp $(INC)/calculadorArea.h
		$(CC) $(CPPFLAGS) -c $(SRC)/calculadorArea.cpp -o $(BUILD)/calculadorArea.o

	$(BUILD)/circuloMain.o: $(SRC)/circuloMain.cpp $(INC)/calculadorArea.h
		$(CC) $(CPPFLAGS) -c $(SRC)/circuloMain.cpp -o $(BUILD)/circuloMain.o

	$(BUILD)/trianguloMain.o: $(SRC)/trianguloMain.cpp $(INC)/calculadorArea.h
		$(CC) $(CPPFLAGS) -c $(SRC)/trianguloMain.cpp -o $(BUILD)/trianguloMain.o

	$(BUILD)/retanguloMain.o: $(SRC)/retanguloMain.cpp $(INC)/calculadorArea.h
		$(CC) $(CPPFLAGS) -c $(SRC)/retanguloMain.cpp -o $(BUILD)/retanguloMain.o

clean:
	rm -f $(BIN)/*
	rm -f $(BUILD)/*