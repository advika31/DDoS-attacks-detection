# Quantum Machine Learning for DDoS Attack Detection

This repository contains all source code, data preprocessing pipelines, and model architectures used for the experiments in the paper:

> **Quantum Machine Learning for Intrusion Detection of Distributed Denial of Service Attacks: A Comparative Overview**  
> DOI: [https://doi.org/10.1117/12.2593297](https://doi.org/10.1117/12.2593297)

## Overview

We demonstrate and benchmark hybrid quantum-classical (PyTorch + PennyLane) machine learning models for detecting Distributed Denial of Service (DDoS) attacks in network traffic datasets. Our workflow includes feature extraction, data preprocessing (scaling, PCA), quantum circuit simulation, model evaluation, and results visualization.

## Key Features

- **Full preprocessing pipeline**: From raw CSV to scaled, PCA-reduced, and cleaned tensors.
- **Hybrid Quantum Neural Network**: PyTorch + Pennylane `TorchLayer` implementation, easily switchable to classical baselines.
- **Works on large real-world datasets**: Easily processes the CIC DDoS 2019 dataset from UNB.
- **Extensive EDA and visualizations**: For insights into dataset structure and feature separability.
- **Automatic metrics and confusion matrix analysis**: Using scikit-learn for unbiased evaluation.
- **Easy-to-use, modular code**: Adaptable for both classical and quantum models.

## Getting Started

### 1. Requirements

- Python 3.8+
- PyTorch
- PennyLane (`pip install pennylane`)
- scikit-learn
- numpy, pandas, seaborn, matplotlib

Install them with:
```bash
pip install torch pennylane scikit-learn pandas numpy matplotlib seaborn
```

### 2. Dataset

The experiments use the open **CIC DDoS 2019** dataset from the University of New Brunswick:

- [Dataset Download Link](https://www.unb.ca/cic/datasets/ddos-2019.html)

### 3. Running the Experiments

**Typical workflow in a Jupyter notebook or script:**
1. Load and preprocess data: Select numeric features, clean, scale, PCA.
2. Initialize and train the model using provided hybrid model code.
3. Evaluate on held-out test data using the detailed metrics pipeline.
4. Generate EDA and plots for insights.

## References and Acknowledgements
- Data: [CIC DDoS 2019 Dataset, UNB](https://www.unb.ca/cic/datasets/ddos-2019.html)
