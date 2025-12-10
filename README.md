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
