Before starting any DFT calculation on a new structure or system you need to make sure you have a robust Input file. 

This means optimising for the K-point grid to minimize integration errors, picking up the suitable energy and density cutoffs for the plane wave expansion and choosing a suitable scf convergence. 

see the lecture notes for more details. 

This hands on is accompanied with an in class group activity (a micro-project)

# The in-class micro project hands on:

In DFT calculations, we need well converged calculations, i.e, ones where the numerical solution accurately enough approximates the true solution of the mathematical problem with a specific exchange-correlation functional. Here we want to see how we can converge to a solution. There are two kinds of convergences, one is for the specific calculation of the total energy, and the other is for specific properties, which may be band structure or defect energies (i.e more of a difference in energy rather than absolute value of the energy).

1. The original files have a very high SCF convergence of $conv_thr=1e-8$, change this to $1e-4$ and run both part 1 and part 2 (see file) until you think you have a convergence in $E_tot$ for k-point and $E_{cut}$. 

2. lower the density convergence threshold even further, compare the results 

3. **Cancellation of errors:** we will devide into groups of students, each about 4, with one raporteaur. Each group will focus on a different set of k-point, Ecut and $\delta v$, and calculate $\delta E$ between a system with $a0=3.615 $\AA and one with $a_1 = a_0*1.1$, does the difference in energy converge faster than the total energy?


A good source reading is the book by [Sholl and Steckel, Density Functional Theory See UCL Library](https://onlinelibrary.wiley.com/doi/book/10.1002/9780470447710)

below is an excerpt from Chapter 3 which is very useful for this excercise. 

1. Before pursuing a large series of DFT calculations numerical convergence of the calculations with respect to the number of k points, Ecut and threshold should be done.  
2. Always report which k points, Ecut and threshold, and PP used as this makes reproduction of the result possible.  
3. Increasing the volume of a supercell reduces the number of k points needed to achieve convergence because volume increases in real space correspond to volume decreases in reciprocal space.  
4. If calculations involving supercells with different volumes are to be compared, choosing k points so that the density of k points in reciprocal space is comparable for the different supercells is a useful way to have comparable levels of convergence in k space.  
5. Understanding how symmetry is used to reduce the number of k points for which calculations are actually performed can help in understanding how long individual calculations will take. 
