# iPIC3D
A massively parallel implementation of implicit Particle-in-Cell method for plasma simulations

## Compile
create a build directory (e.g., build) and call CMake. Upon completion, executable iPIC3D* and library libiPIC3Dlib.a should be generated in the build folder.
```bash
mkdir build
cd build
cmake ..
make -j
```

## Run
iPIC3D uses MPI for parallel execution. Ensure number_of_MPI_processes = XLEN x YLEN x ZLEN in the input file.
```bash
mpirun -n number_of_MPI_processes ./iPIC3D input_file.inp
```
