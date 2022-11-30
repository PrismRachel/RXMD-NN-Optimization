# Robust Multiscale Neural Network Quantum Molecular Dynamics for Emerging Topotronics

## Project description
Neural network quantum molecular dynamics (NNQMD) simulations based on machine learning (ML) will dominate atomistic modeling of materials in this century by achieving quantum-mechanical accuracy at a drastically reduced computational cost. The current roadblocks that prevent large NNQMD simulations at the scale of optoelectronic device structures are: 
(1) scaling problem that even exascale computers cannot model realistic device structures; 
(2) fidelity-scaling problem, in which accumulation of model error causes breakdown of large spatiotemporal simulations. 

## Methods and approach
(1) a multiscale neural-network (NN)/molecular-mechanics (MM) approach that embeds compute-intensive NNQMD simulation in low-cost MM-based molecular dynamics simulation only when and where high fidelity is needed;
(2) sharpness regularization to make simulations robust against fidelity-degrading thermal noise. 
(3) parallel implementation of our NNQMD algorithm as well as performance optimization on graphics processing unit (GPU).

	
## The current progress
The code has achieved a parallel efficiency of 0.98 for 5.2-billion atom system on 262,144 cores of the Theta supercomputer at Argonne Leadership Computing Facility (ALCF). In preparation for the forthcoming ALCF Aurora exascale computer, we have offloaded key kernels of the NNQMD code to graphics processing units, gaining 4.36-5.34x speedup, and additional 1.7x speedup by loop reordering. 


<img width="486" alt="image" src="https://user-images.githubusercontent.com/38379489/204931385-08bae7ff-f0d1-48f4-abad-53c84a085a28.png">


## Expectations
The resulting NNQMD code will enable first simulation of strain-induced skyrmion-to-skyrmionium topological transition toward achieving ultralow-power opto-topotronic devices. 

