# Poisson2d_parallel
Numerical solution a 2D poisson's equation with Dirichlet Boundary conditions. PETSc krylov subspace solver routines were implemented in c in order to numerically solve the arising linear system of equations after the PDE was discretized. PETSc supports MPI and thus allows solving the system using parallel processing. The command line arguments passed to the code include the size of the rectangular grid, the KSP solver and preconditioner to be used.

Numerical experiments were performed to do speed-up tests in order to understand the how run-times are affected when the number of processors are increased for a particular grid size. This was done for each different rectangular grid size, starting with 2^5 x 2^5 up to 2^10 x 2^10.
