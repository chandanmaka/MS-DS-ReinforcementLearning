## CartPole-v1 Algorithm Comparison (Lab 8)

This lab investigates how three different reinforcement learning methods perform on the `CartPole-v1` control task:

- **Tabular Q-Learning** with discretized continuous states  
- **SARSA with Tile Coding** for function approximation  
- **REINFORCE with a learned baseline** implemented in PyTorch

All code lives in the notebook `Week_8_assignment.ipynb`, which contains:

- Problem description and environment inspection  
- Implementations of the three agents  
- Training loops and evaluation  
- Plots of learning curves and final performance, plus a brief written comparison

### 1. Environment and dependencies

The notebook assumes:

- **Python** ≥ 3.9  
- Access to **Jupyter Notebook** or **JupyterLab**

Python dependencies are listed in `requirements.txt` and include:

- `gymnasium[classic-control]` for the CartPole environment  
- `torch` for the REINFORCE agent and baseline network  
- `numpy`, `pandas` for numerical work and tabular summaries  
- `matplotlib` for plotting

### 2. Setup

From this `Lab8` directory:

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

If you already have a course environment with these packages installed, you may skip the virtual environment and installation steps.

### 3. Running the notebook

1. Start Jupyter from the `Lab8` directory:

   ```bash
   jupyter notebook
   ```

2. Open `Week_8_assignment.ipynb`.
3. Run all cells (Kernel → Restart & Run All) or execute them sequentially from top to bottom.

The notebook will:

- Train each of the three algorithms on `CartPole-v1` using several random seeds  
- Plot learning curves with error bands  
- Plot a final performance comparison with error bars  
- Summarize the trade‑offs between the methods (sample efficiency, stability, implementation complexity, etc.)

### 4. Reproducing or modifying experiments

- **Hyperparameters** such as learning rates, exploration schedules, and network sizes are defined in the notebook and can be edited directly to run alternative configurations.  
- **Random seeds** are also controlled in the notebook to support basic reproducibility; you can adjust the seed list to run more or fewer repeats.  
- To adapt this work to other classic-control tasks (e.g., `MountainCar-v0`), change the `gymnasium` environment ID and, if needed, update discretization or tile-coding settings.

### 5. File summary

- `Week_8_assignment.ipynb` – main lab notebook with code, experiments, and analysis.  
- `requirements.txt` – Python dependencies used by the notebook.

