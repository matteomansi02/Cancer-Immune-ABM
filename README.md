### Overview
This repository contains a simulation of cancer cell growth in a spatial grid and its interaction with T-cells using the Agentpy library. The simulation also incorporates the diffusion equation to model oxygen distribution, which is essential for cancer cell survival and replication, as well as the IL-2 cytokine, which is utilized by T-cells for activation.
Current research in cancer modeling and simulation focuses on understanding the spatiotemporal behavior of cancer cells and their interactions with immune cells, such as T-cells. Agent-based models (ABMs) have gained popularity in this domain due to their ability to represent individual cells as agents and capture heterogeneous behaviors. 

### Simulation Algorithm
The simulation algorithm can be summarized as follows:

1. Initialize the spatial grid with 1 cancer cell, and oxygen and IL-2 cytokine distributions.
2. Calculate the diffusion of oxygen and IL-2 cytokine using the diffusion equation to model their spatial distributions.
3. Determine the effects of oxygen concentration on cancer cell proliferation and apoptosis.
4. Update the positions and states of cancer cells and T-cells based on their rules of movement, proliferation, and interactions.
5. Repeat the process until the simulation time is reached.

### Usage
Clone this repository and run the main simulation script to observe the cancer cell growth and T-cell interactions. 
I used IPython for animation in jupyter.
Using the agentpy.animate function, the code will plot 3 animations in parallel, the one with cells, the one of oxygen diffusion and the one of IL-2 diffusion.
The parameters are all in a commented dictionary, and are changed manually.
For shorter simulation times, I recommend decreasing the Tmin parameter.
The number of iterations is given by the step parameter.

### References
This simulation is inspired by various research studies and computational models in the field of cancer biology and immunology. 

[On-lattice agent-based simulation of populations of cells within the open-source Chaste framework](https://royalsocietypublishing.org/doi/full/10.1098/rsfs.2012.0081)

[A computational multiscale agent-based model for simulating spatio-temporal tumor immune response to PD1 and PDL1 inhibition](https://royalsocietypublishing.org/doi/full/10.1098/rsif.2017.0320#RSIF20170320F2)
