all: main

clean:
	rm -rf *.a *.h main *.a

sdlgotest.a:
	go build -buildmode=c-archive -o sdlgotest.a main.go

main: sdlgotest.a
	gcc main.c sdlgotest.a -o main -lpthread
