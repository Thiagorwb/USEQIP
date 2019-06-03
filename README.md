# USEQIP
These are the Qiskit coding projects/experiments I ran during the USEQIP program at the IQC at UWaterloo, Summer 2019.

## Max-Cut

The Max-Cut project is my implementation of the Quantum Approximate Optimization Algorithm on the Max-Cut problem as a quantum subroutine of an unsupervised learning algorithm. The project is based off of the paper by the Rigetti Computing Group, "Unsupervised Machine Learning on a Hybrid Quantum Computer".

In particular, the QAOA is a short-depth circuit; 2 CNOT gates per adjacent edge of the maximum out-degree vertex, parametrized by a set of angles {gamma_i, beta_i}. I then use Bayesian Optimization to maximize the resulting cut by optimize over the choice of angles. I use the Bayesian_Optimization python package to do so. 

