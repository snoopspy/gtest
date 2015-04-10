.PHONY: all cmake build install uninstall

all: cmake build install

cmake:
	cmake ..

build:
	make -f Makefile

install:
	cp gtest.pri ..
	sudo cp -r ../include/gtest /usr/local/include/gtest
	sudo cp libgtest.a /usr/local/lib/libgtest.a
	sudo cp libgtest_main.a /usr/local/lib/libgtest_main.a
	
uninstall:
	rm -f ../gtest.pri
	sudo rm -rf /usr/local/include/gtest
	sudo rm -f /usr/local/lib/libgtest.a
	sudo rm -f /usr/local/lib/libgtest_main.a
