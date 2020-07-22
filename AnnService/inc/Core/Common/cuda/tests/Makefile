ARCH=sm_70

CUDA_HOME=/usr/local/cuda
FLAGS=-std=c++14 -Xptxas -O3

all: unitTests

unitTests: unitTests.cu ../Distance.hxx
	nvcc ${FLAGS} --use_fast_math --gpu-architecture=${ARCH} -o unitTests unitTests.cu
