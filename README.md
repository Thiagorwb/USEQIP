# USEQIP
These are the Qiskit coding projects/experiments I ran during the USEQIP program at the IQC at UWaterloo, Summer 2019.

## Max-Cut

The Max-Cut project is my implementation of the Quantum Approximate Optimization Algorithm [1] on the Max-Cut problem as a quantum subroutine of an unsupervised learning algorithm. The project and implementation is based off of a recent paper by the Rigetti Computing Group [2].

In particular, the QAOA is a short-depth circuit; 2 CNOT gates per adjacent edge of the maximum out-degree vertex, parametrized by a pair of angles \gamma, \beta. After running and measuring the circuit for some number of shots, each bitstring measured is mapped to a cut (S, V\S), over which the maximum correspondent cut value is returned. Bayesian Optimization is then used to maximize the resulting cut value by optimizing over the choice of angles. I use the BayesianOptimization python package [3] to do so. 

[1] E. Farhi, J. Goldstone, S. Gutmann e-print arXiv 1411.4028 (2014)

[2] Rigetti Computing, 'Unsupervised Machine Learning on a Hybrid Quantum Computer' (2017)

[3] https://github.com/fmfn/BayesianOptimization
