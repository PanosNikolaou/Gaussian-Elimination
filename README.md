# Gaussian elimination in Fortran

A small Fortran example solving a linear system `Ax = b` using Gaussian elimination and back substitution. The example matrix and right-hand side are defined in `main.f90`, and the solution is printed to the terminal.

## Build and run

Install GNU Make and `gfortran`, then run:

```sh
make
./gauss
```

Edit the matrix, vector, and dimension in `main.f90` and rebuild to experiment with another system. `functions.f90` and `tools.f90` provide numerical and supporting routines; `types.f90` defines numerical types. `make clean` removes generated object and module files.

This is an educational example. Check the implementation's assumptions and numerical behavior for singular or ill-conditioned systems before using it for other inputs.
