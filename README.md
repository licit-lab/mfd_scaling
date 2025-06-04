# mfd_scaling: Hierarchical Scaling and Variogram-based Imputation

This repository contains the Python notebooks and code used in the paper:
**"Scaling Methods for Estimating Macroscopic Fundamental Diagrams in Urban Networks with Sparse Stationary Sensor Coverage"**.

The repository provides two main components:
- **Hierarchical Scaling**: A method for scaling traffic variables from an LD-equipped subnetwork to non-equipped links using road hierarchy information.
- **Variogram-based Imputation**: A geostatistical approach for estimating missing traffic states based on spatial dependencies captured by empirical variograms.

![[Variogram](https://github.com/licit-lab/mfd_scaling/main/pictures/variogram.jpg?raw=true)](https://github.com/licit-lab/mfd_scaling/blob/main/pictures/variogram.jpg)

![Hierarchical Scaling results](https://github.com/licit-lab/mfd_scaling/blob/main/pictures/eq_neq_flow.jpg)

## Contents

- `hierarchical_scaling.ipynb`: Jupyter Notebook demonstrating the hierarchical scaling methodology, including:
  - Link hierarchy classification
  - Scaling factor estimation
  - Network-wide traffic state extrapolation

- `variogram.ipynb`: Jupyter Notebook implementing the variogram-based imputation approach, including:
  - Empirical variogram estimation
  - Model fitting and parameter calibration
  - Kriging interpolation for traffic state imputation

## Requirements

The notebooks are written in Python 3 and require the following packages:

- `numpy`
- `pandas`
- `matplotlib`
- `scikit-learn`
- `scikit-gstat`
- `networkx` (for graph-based distance calculations)
- `geopandas` (optional, for visualizing spatial data)

Install dependencies via:

```bash
pip install -r requirements.txt
