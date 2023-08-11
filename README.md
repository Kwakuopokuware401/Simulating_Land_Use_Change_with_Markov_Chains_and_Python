# Simulating_Land_Use_Change_with_Markov_Chains_and_Python

This project implements a simple Markov chain model to simulate land use change over time. It generates random transition probability matrices and initial land cover maps, then iterates through time steps to transition each cell to a new land cover class based on the Markov transition probabilities.


![markov_chain](https://github.com/Kwakuopokuware401/Simulating_Land_Use_Change_with_Markov_Chains_and_Python/assets/94206249/3b18fe84-4e97-4bd9-9a0e-b2d0534309ba)

Author: Kwaku Opoku-Ware (kwakuopokuware401@gmail.com)


# Usage
The key parameters to modify are:
- NUM_TIMESTEPS - number of time steps to simulate

- LANDCOVER_CLASSES - list of land cover class names

# Code overview

- TRANSTION_PROBS - 3D array of transition probability matrices for each time step

- INIT_MAP - Randomly generated initial land cover map

- cur_map - Land cover map for current time step

 - next_map - Land cover map for next time step

 ## Inside loop:

- Apply mask where cur_map equals current land cover class

- Get transition probabilities for that class

- Randomly choose new class for each cell based on probabilities

- Update next_map with new classes

- Plot initial and final maps

# Requirements

- Numpy

- Matplotlib
