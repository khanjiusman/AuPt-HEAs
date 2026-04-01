This repository contains code that is an adapted and modified implementation of the Deep Reinforcement Learning (DRL) framework originally developed in:

J. Phys. Chem. A, 2024, 128, 42, 9122–9134.

We gratefully acknowledge the original authors for developing the methodology, which has been extended and customized in this project for application to quaternary Au–Pt-based high-entropy alloy nanoclusters.

### How to Run the Code

1. **Set Up the Environment:**
   - Install the required Conda environment using the provided YAML file:
     ```bash
     conda env create -f env_clusgym.yml
     ```

2. **Configure the Nanocluster Composition:**
   - Edit `gym_trpo_parallel.py` or `gym_trpo_single.py` to select the desired nanocluster composition.
	- For simulating a high entropy alloy AuPtNiCu cluster of 12 atoms:
     ```python
     eleNames = ['Au', 'Pt', 'Ni', 'Cu']
     eleNums = [3,3,3,3]
     ```
    - For simulating a high entropy alloy AuPtPdCu cluster of 12 atoms:
     ```python
     eleNames = ['Au', 'Pt', 'Pd', 'Cu']
     eleNums = [3,3,3,3]
     ```
	- For simulating a high entropy alloy AuPtPdNi cluster of 12 atoms:
     ```python
     eleNames = ['Au', 'Pt', 'Pd', 'Ni']
     eleNums = [3,3,3,3]
     ```

	- For simulating a high entropy alloy AuPtPdAg cluster of 8 atoms:
     ```python
     eleNames = ['Au', 'Pt', 'Pd', 'Ag']
     eleNums = [2,2,2,2]
     ```

	- For simulating a high entropy alloy AuPtPdAg cluster of 12 atoms:
     ```python
     eleNames = ['Au', 'Pt', 'Pd', 'Ag']
     eleNums = [3,3,3,3]
     ```

	- For simulating a high entropy alloy AuPtPdAg cluster of 20 atoms:
     ```python
     eleNames = ['Au', 'Pt', 'Pd', 'Ag']
     eleNums = [5,5,5,5]
     ```


3. **Run the Simulation:**
   - Execute the script using Python. Choose the appropriate version for your needs:
     ```bash
     python gym_trpo_single.py    # For single execution
     ```
---
# Note
The code is adapted from [**clusgym_drl**](https://github.com/rajeshkochi444/clusgm_drl). We thank the authors for making the code available on github.
