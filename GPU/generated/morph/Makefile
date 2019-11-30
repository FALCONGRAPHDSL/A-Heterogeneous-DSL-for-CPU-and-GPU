TOPLEVEL := ../../..
APP=morph
NVCC=/usr/local/cuda/bin/nvcc
all:
	$(NVCC) -O3   -I ./dmrheader falcondmr.cu -o dmr
	cp dmr $(TOPLEVEL)/bin/GPU/morph/
	$(NVCC) -O3   -I ../include dynamicsssp.cu -o dynamicsssp
	cp dynamicsssp $(TOPLEVEL)/bin/GPU/morph/
