FORT = gfortran -std=legacy
CFLAGS = -c

all: test_install polsys_plp.o lapack_plp.o
	./test_install

test_install: test_install.f90 polsys_plp.o lapack_plp.o
	$(FORT) test_install.f90 polsys_plp.o lapack_plp.o -o test_install

polsys_plp.o: polsys_plp.f90
	$(FORT) $(CFLAGS) polsys_plp.f90 -o polsys_plp.o

lapack_plp.o: lapack_plp.o
	$(FORT) $(CFLAGS) lapack_plp.f -o lapack_plp.o

clean:
	rm -f test_install polsys_plp.o lapack_plp.o *.mod
