## Parallelisation
(Course: High Performance Computing for Mathematicians)

This repository contains two assignments with C++ code parallelised using MPI, along with two reports, namely 

- Parallel 1D heat equation, and

- Parallel 2D wave equation.

The 2D wave equation folder contains three different approaches towards parallelisation (horizontal and vertical stripes, and squares), further described in the report located in the folder.

The parallel code was run on Cirrus. The compiler files are named `compile_now`, and the jobs were submitted using the slurm files `run_job.slurm`.

Instead of using a supercomputer like Cirrus, the scripts can also be ran locally, for example with `OpenMPI` the code can be compiled by typing 

`mpicxx <name_file.cpp> -o exe` 

in the terminal, where `<name_file.cpp>` should be replaced by the corresponding file name, and then ran by

`mpirun -np N exe`

where `N` is the number of processors you wish to employ.
