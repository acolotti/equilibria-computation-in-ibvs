# Systems of equations and numerical results for the article "Determination of All Stable and Unstable Equilibria for Image Points-Based Visual Servoing", submitted to IEEE T-RO

## Systems of equations

In this folder, you can find the systems corresponding to each test case presented in Section IV, as well as the symmetry-invariant change of variables presented in Section III-B (for the 4 points case only).

In each file, the first line denotes the system's variables, the second line is the characteristic of the field over which the computations are performed, and the subsequent lines represent the actual system of equations.

These systems are meant to be solved with `msolve` [https://msolve.lip6.fr], which is an open-source, high-performance library for computing the real roots of zero-dimensional polynomial systems that relies on Gröbner bases algorithms.

Once `msolve` is installed, it's possible to solve a system by launching the following command:
```console
./msolve -f Case_XY.sys -o Case_XY.sols
```
The solutions will be saved in the `Case_XY.sols` file. The `msolve` executable is located in the `/msolve_installation/binary` folder.

## Numerical solutions

In this folder, you can find the numerical solutions (approximated to the nearest thousandth) for all the test cases presented in Section IV, expressed in camera state-space.
