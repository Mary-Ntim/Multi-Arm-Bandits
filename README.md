# Multi-Armed Bandit Algorithms: A Comparative Study
This repository contains a comprehensive implementation and evaluation of several foundational algorithms used for solving the multi-armed bandit problem. The objective is to compare how different exploration strategies perform under both stationary and non-stationary reward settings. The experiments were conducted as part of an academic assignment in reinforcement learning.

---

## Overview

The following algorithms were implemented from scratch and evaluated:

- **Greedy** (with non-optimistic initial values)
- **Epsilon-Greedy** (with parameter tuning via pilot runs)
- **Optimistic Greedy** (using high initial estimates)
- **Gradient Bandit** (with learning rate α tuned via pilot runs)

Performance was measured using:

- The **average reward per time step**
- The **proportion of time the optimal action** was selected

Each algorithm was evaluated over **1000 simulations** of **2000 time steps** each. For reproducibility, separate independent random streams were used across simulations.

---

## Setup

This project is designed to run in [Google Colab](https://colab.research.google.com/) or a Python 3.x environment.


### Reproducing the Results

To exactly reproduce the figures in this report:

1. Clone the repository.
2. Run all cells in `Multi_Arm_Bandit_Code.ipynb` without modifying any parameters.
4. The plots for average reward and optimal action selection will be saved or displayed automatically.
5. Random seeds and experimental configurations are fixed to ensure replicability across runs.

No GPU or external data is required.

### Reproducibility Details

All experiments use:
- Fixed NumPy seeds for each simulation (to ensure independence and consistency)
- Shared drift/permutation configurations for non-stationary settings
- Identical reward initialization across algorithms in each trial

This ensures fair comparison and supports full experimental reproducibility, in line with ML research standards.
