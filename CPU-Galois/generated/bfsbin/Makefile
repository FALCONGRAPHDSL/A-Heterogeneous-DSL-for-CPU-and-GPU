TOPLEVEL := ../../..
APP=bfsbin
GCC=g++
include ../../common.mk
all:
	$(GCC) -c  -I$(GALOIS_ROOT)/include/ -I $(GALOIS_ROOT)/build/default/include/ -L$(GALOIS_ROOT)/build/default/lib/libgalois.a -O3 -std=c++11 -D__STDC_CONSTANT_MACROS -D__STDC_LIMIT_MACROS  -fopenmp -lgomp  -w  -fpermissive bfscoll.cpp  -o xxss
	$(GCC)  xxss $(GALOIS_ROOT)/build/default/src/libgalois.a -lpthread -fopenmp -o bfs
	mv bfs $(TOPLEVEL)/bin/CPU-Galois/bfs/bfs
