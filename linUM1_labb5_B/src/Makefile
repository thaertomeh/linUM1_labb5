all: main.o my_add.o main
	echo "all running linking and compiling files"
		
main.o: main.c my_add.h
	gcc -c main.c 
my_add.o: my_add.c my_add.h
	gcc -c my_add.c 
main:  main.c my_add.c 
	gcc main.c my_add.c -o main 
install:
	sudo install ./main.c //usr/bin
	sudo install ./my_add.c //usr/bin
	sudo install ./my_add.h //usr/bin	
	sudo install ./main //usr/bin	
uninstall:
	sudo rm -rf //usr/bin/*.c 
	sudo rm -rf //usr/bin/*.h
	sudo rm -rf //usr/bin/main
	  
clean:
	rm -rf *o main
