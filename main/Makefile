all: main

clean:
	rm -rf *.a *.h main *.so

sdlgotest.so:
	go build -buildmode=c-shared -o sdlgotest.so main.go

main: sdlgotest.so
	gcc main.c ./sdlgotest.so -o main
