# RXMD-NN-Optimization
## Project description
Neural network quantum molecular dynamics (NNQMD) simulations based on machine learning will dominate atomistic modeling of materials in this century by achieving quantum-mechanical accuracy at a drastically reduced computational cost. Despite enormous successes, there remain several roadblocks that prevent large NNQMD simulations at the scale of optoelectronic device structures: 
(1) scaling problem that even exascale computers cannot model realistic device structures; 
(2) fidelity-scaling problem, in which accumulation of model error causes breakdown of large spatiotemporal simulations. 

## Methods and approach
(1) a multiscale neural-network (NN)/molecular-mechanics (MM) approach that embeds compute-intensive NNQMD simulation in low-cost MM-based molecular dynamics simulation only when and where high fidelity is needed;
(2) sharpness regularization to make simulations robust against fidelity-degrading thermal noise. 
	
## Expectations
The code has achieved a parallel efficiency of 0.98 for 5.2-billion atom system on 262,144 cores of the Theta supercomputer at Argonne Leadership Computing Facility (ALCF). In preparation for the forthcoming ALCF Aurora exascale computer, we have offloaded key kernels of the NNQMD code to graphics processing units, gaining 4.36-5.34x speedup, and additional 1.7x speedup by loop reordering. The resulting NNQMD code has enabled first simulation of strain-induced skyrmion-to-skyrmionium topological transition toward achieving ultralow-power opto-topotronic devices.

