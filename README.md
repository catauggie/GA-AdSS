# Adaptive Search-Space Scaling (AdSS) for Genetic Algorithms

This repository contains the source code, experimental scripts, and visualisation results associated with the study on adaptive search-space scaling for genetic algorithms and self-configuring evolutionary algorithms.

The project investigates a cluster-guided dynamic modification of the search domain based on the Individual Cluster Efficiency (ICE) criterion. The proposed approach is evaluated both for a classical binary-coded Genetic Algorithm (GA) and for a Self-Configuring Genetic Algorithm (SelfCGA), demonstrating improved convergence speed, solution quality, and robustness on multimodal benchmark problems.

---

## 📁 Repository Contents

### 📊 Experimental Results (PDF)
- `D10_curves_ga_.pdf` — Convergence curves for GA and GA with adaptive search-space scaling at \(D=10\)
- `GA_vs_ClusterGA_whiskers_D10_all.pdf` — Boxplots for GA and cluster-guided GA at \(D=10\)
- `D10_curves_selfcga_.pdf` — Convergence curves for SelfCGA and SelfCGA with scaling at \(D=10\)
- `selfcga_vs_ClusterSelfcga_whiskers_D10_all_.pdf` — Boxplots for SelfCGA and its scaled variant at \(D=10\)

- `D30_curves_selfcga_.pdf` — Convergence curves for SelfCGA and scaled SelfCGA at \(D=30\)
- `selfcga_vs_ClusterSelfcga_whiskers_D30_all_.pdf` — Boxplots at \(D=30\)

- `D50_curves_selfcga_.pdf` — Convergence curves for SelfCGA and scaled SelfCGA at \(D=50\)
- `selfcga_vs_ClusterSelfcga_whiskers_D50_all_.pdf` — Boxplots at \(D=50\)

---

### 🧠 Notebooks
- `GA.ipynb` — Baseline classical Genetic Algorithm
- `GA + mode.ipynb` — GA with adaptive search-space scaling (cluster-guided)
- `SelfCGA.ipynb` — Baseline self-configuring genetic algorithm
- `SelfCGA + mode.ipynb` — SelfCGA with adaptive search-space scaling

---

## ⚙️ Requirements

To run the experiments, the following external dependencies are required:

### 1. **CEC 2017 Benchmark Suite (Python implementation)**  
   Required for all test functions:
   > D. T. <CEC 2017 implementation> ([official benchmark package](https://github.com/tilleyd/cec2017-py))

   The functions are expected to be available under:
   ```python
   from cec2017 import basic, transforms
   ```
### 2. thefittest Python library  
Full description on https://github.com/sherstpasha/thefittest. Required for the SelfCGA implementation:

```bash
pip install thefittest
```


### 3. Standard scientific Python stack
```
numpy
scipy
scikit-learn
matplotlib
```
