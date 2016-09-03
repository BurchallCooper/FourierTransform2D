
#CXX      = ~/openmpi/bin/mpic++
CXX	 = /usr/lib64/openmpi/bin/mpic++
#EXX	 = ~/openmpi/bin/mpiexec
EXX	 = /usr/lib64/openmpi/bin/mpiexec
IFILE 	 =  Tower.txt
NPROC	 = 16
#IFILE    = test.32x32.txt
#NPROC    = 4	
CXXFLAGS = -Wall -g

all:	main.cpp  Complex.cc InputImage.cc
	$(CXX)  -g -o fft2d main.cpp Complex.cc InputImage.cc

run: 	
	$(EXX) -n $(NPROC) fft2d $(IFILE)

clean:
	@rm  fft2d *.wbctxt


