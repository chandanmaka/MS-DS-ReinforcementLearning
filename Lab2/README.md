# Week 2 Assignment: Dynamic Programming on GridWorld and FrozenLake

This notebook implements and compares classic dynamic programming methods for solving small Markov Decision Process environments.

## What is in the notebook

The notebook includes:

- a custom **GridWorld** environment written in a Gymnasium-style format
- a helper to extract the full transition model `P(s', r | s, a)`
- **Policy Iteration** in two versions:
  - synchronous policy evaluation
  - in-place policy evaluation
- **Value Iteration** in two versions:
  - synchronous updates
  - in-place updates
- experiments on:
  - deterministic GridWorld
  - stochastic GridWorld
  - Gymnasium **FrozenLake-v1**
- visualizations for:
  - value function snapshots
  - policy snapshots
  - convergence curves
  - compact summary tables

## Main goal

The goal of the assignment is to study how policy iteration and value iteration behave under different transition settings, and to compare convergence speed and final policies in custom GridWorld and FrozenLake.

## Files

- `Week_2_assignment.ipynb` — main notebook
- `requirements.txt` — Python packages needed to run the notebook

## Requirements

Install the dependencies first:

```bash
pip install -r requirements.txt
```

## How to run

1. Open the notebook in Jupyter Notebook, JupyterLab, or VS Code.
2. Install the required packages.
3. Run the cells from top to bottom.

## Libraries used

- `numpy`
- `matplotlib`
- `gymnasium`
- `time` (Python standard library)

## Notes

- The notebook uses **NumPy arrays** for value functions and policies.
- FrozenLake experiments require `gymnasium` to be installed.
- The notebook includes both deterministic and stochastic transition settings for comparison.
