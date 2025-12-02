Before starting any DFT calculation on a new structure or system you need to make sure you have a robust Input file. 

This means optimising for the K-point grid to minimize integration errors, picking up the suitable energy and density cutoffs for the plane wave expansion and choosing a suitable scf convergence. 

see the lecture notes for more details. 

This hands on is accompanied with an in class group activity (a micro-project)

# the class micro project:

Usually in DFT calculations, well-converged” calculation is one in which the numerically derived solution accurately approximates the true solution of the mathematical problem posed by DFT with a specific exchange –correlation functional.The concept of numerical convergence is quite separate from the question of whether DFT accurately describes physical reality.

1. The original files have a very high SCF convergence of $1e-8$, change this to $1e-4$ and run both part 1 and part 2 until you think you have a convergence in $E_tot$ for k-point and $E_{cut}$. 

2. lower teh density convergence threshold even further, compare the results 

3. Cancellation of errors: we will devinde into groups, each group will focus on a different set of k-point, Ecut and $\delta v$, and calculate $\delta E$ between a system with $a0=3,615 $\AA and one with $a_1 = a_0*1.1$, does the difference in energy converge faster than the total energy?


A good source reading is the book by [Sholl and Steckel, Density Functional Theory See UCL Library](https://onlinelibrary.wiley.com/doi/book/10.1002/9780470447710)

below is an excerpt from Chapter 3 which is very useful and important! 

1. Before pursuing a large series of DFT calculations for a system of interest, numerical data exploring the convergence of the calculations with respect to the number of k points should be obtained.  
2. The number of k points used in any calculation should be reported since not doing so makes reproduction of the result difficult.  
3. Increasing the volume of a supercell reduces the number of k points needed to achieve convergence because volume increases in real space correspond to volume decreases in reciprocal space.  
4. If calculations involving supercells with different volumes are to be compared, choosing k points so that the density of k points in reciprocal space is comparable for the different supercells is a useful way to have comparable levels of convergence in k space.  
5. Understanding how symmetry is used to reduce the number of k points for which calculations are actually performed can help in understanding how long individual calculations will take. 

Overall convergence is determined by the density of k points in the full Brillouin zone, not just the number of k points in the irreducible Brillouin zone.  6. Appropriate methods must be used to accurately treat k space for metals.