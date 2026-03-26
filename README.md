# Graph-Based Deep Learning for Intelligent Detection of Energy Losses, Theft, and Operational Inefficiencies in Oil & Gas Production Networks

![arXiv](https://img.shields.io/badge/arXiv-2603.14406-b31b1b.svg)
![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Research](https://img.shields.io/badge/Type-Research-green.svg)

This repository contains the implementation of the research paper:

**Graph-Based Deep Learning for Intelligent Detection of Energy Losses, Theft, and Operational Inefficiencies in Oil & Gas Production Networks**

Preprint available on arXiv:
https://arxiv.org/abs/2603.14406

---

## Overview

Early detection of energy losses, theft, and operational inefficiencies is a major challenge in oil and gas production systems due to complex interactions between wells, facilities, and production infrastructure. Traditional machine learning models typically treat wells or sensors independently and therefore fail to capture system-wide dependencies.

This project proposes a **spatiotemporal graph-based deep learning framework** that models oil and gas production systems as **interconnected networks**. By combining **temporal sequence learning** with **graph neural networks**, the approach captures both **temporal dynamics** and **relational dependencies** among production assets.

The framework enables improved detection of abnormal production behavior such as:

* Energy losses
* Production inefficiencies
* Equipment malfunctions
* Potential theft or leakage events

---

## Key Contributions

* Introduces a **graph-based representation** of oil and gas production networks including wells, facilities, and fields.
* Combines **temporal modeling** with **graph attention networks** for anomaly detection.
* Implements **weakly supervised labeling** based on domain-informed heuristics derived from production and pressure behavior.
* Evaluates the framework using **time-based data splits** to simulate real-world deployment conditions.
* Demonstrates improved anomaly detection performance compared with traditional machine learning and sequence-only models.

---

## Methodology

The proposed framework integrates four main components.

### 1. Feature Engineering

Domain-informed features derived from production data including:

* Production rate
* Pressure indicators
* Flow behavior characteristics
* Operational indicators

### 2. Weak Supervision

Because labeled anomaly data in oil and gas operations is limited, domain-informed heuristics are used to construct weak anomaly labels from production and pressure patterns.

### 3. Graph Construction

The production system is represented as a graph where:

* **Nodes** represent wells and facilities
* **Edges** represent production flow relationships
* Additional connections capture wells sharing common infrastructure

### 4. Spatiotemporal Learning

The framework integrates:

* Temporal sequence modeling
* Graph Attention Networks (GAT)
* Joint learning of temporal and relational dependencies

---

## Repository Structure

```
oil-gas-anomaly-detection-gnn/

├── dataset/
│   └── Volve production_data.xlsx

├── Graph_Anomaly_Detection.ipynb
│   # Main Jupyter notebook containing data processing,
│   # graph construction, model training, and evaluation

└── README.md
```

---

## Usage

### 1. Clone the repository

```
git clone https://github.com/abdulqoyumadegoke/oil-gas-anomaly-detection-gnn.git
```

### 2. Navigate into the project directory

```
cd oil-gas-anomaly-detection-gnn
```

### 3. Launch Jupyter Notebook

```
jupyter notebook
```

### 4. Run the notebook

Open:

```
Graph_Anomaly_Detection.ipynb
```

The notebook contains the full pipeline including data preprocessing, graph construction, model training, and anomaly detection evaluation.

---

## Results

Experimental evaluation shows that incorporating both **temporal dynamics and relational dependencies** significantly improves anomaly detection performance.

Under **time-based evaluation**:

* **ROC-AUC ≈ 0.98**
* **Anomaly Recall > 0.93**

The results demonstrate that combining **temporal modeling with graph-based relational learning** improves robustness and detection capability in complex oil and gas production networks.

---

## Citation

If you use this work in your research, please cite:

```
@article{oguntola2026graph,
  title={Graph-Based Deep Learning for Intelligent Detection of Energy Losses, Theft, and Operational Inefficiencies in Oil & Gas Production Networks},
  author={Oguntola, Adewale U. and Olowookere, AbdulQoyum A. and Kolade, Abimbola D.},
  journal={arXiv preprint arXiv:2603.14406},
  year={2026}
}
```

---

## Applications

The framework can be applied to:

* Oil and gas production monitoring
* Pipeline anomaly detection
* Industrial Internet of Things monitoring
* Energy infrastructure analytics
* Smart production optimization systems

---

## License

This repository is provided for **academic and research purposes**.
