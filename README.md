# Graph-Based Deep Learning for Intelligent Detection of Energy Losses, Theft, and Operational Inefficiencies in Oil & Gas Production Networks

This repository contains the implementation of the research paper:

**Graph-Based Deep Learning for Intelligent Detection of Energy Losses, Theft, and Operational Inefficiencies in Oil & Gas Production Networks**

Preprint available on arXiv:  
https://arxiv.org/abs/2603.14406

---

## Overview

Early detection of energy losses, theft, and operational inefficiencies is a major challenge in oil and gas production systems due to complex interactions between wells, facilities, and production infrastructure. Traditional machine learning models typically treat wells or sensors independently and therefore fail to capture system-wide dependencies.

This project proposes a **spatiotemporal graph-based deep learning framework** that models oil and gas production systems as **interconnected networks**. By combining **temporal sequence learning** with **graph neural networks**, the proposed approach captures both **temporal dynamics** and **relational dependencies** among production assets.

The framework enables improved detection of abnormal production behavior, including:

- Energy losses  
- Production inefficiencies  
- Equipment malfunctions  
- Potential theft or leakage events  

---

## Key Contributions

- Introduces a **graph-based representation** of oil and gas production networks including wells, facilities, and fields.
- Combines **temporal modeling** with **graph attention networks** for anomaly detection.
- Implements **weakly supervised labeling** based on domain-informed heuristics derived from production and pressure behavior.
- Evaluates the framework using **time-based data splits** to simulate real-world deployment conditions.
- Demonstrates improved anomaly detection performance compared with traditional machine learning and sequence-only models.

---

## Methodology

The proposed framework integrates four major components:

### 1. Feature Engineering
- Production rate  
- Pressure indicators  
- Flow behavior features  
- Operational indicators  

### 2. Weak Supervision
Domain-informed heuristics are used to generate anomaly labels when labeled anomaly datasets are limited.

### 3. Graph Construction
- Nodes represent wells and facilities  
- Edges represent production flow relationships  
- Additional connections are created among wells sharing infrastructure

### 4. Spatiotemporal Learning
The model integrates:

- Temporal sequence modeling  
- Graph Attention Networks (GAT)  
- Joint learning of temporal and relational dependencies

---

## Repository Structure

```
oil-gas-anomaly-detection-gnn/
│
├── data/                 # Dataset 
├── notebooks/            # Jupyter notebooks for experiments
├── src/                  # Core implementation
│   ├── data_processing.py
│   ├── graph_model.py
│   ├── training.py
│   └── evaluation.py
│
├── results/              # Model outputs
├── figures/              # Plots and figures from experiments
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/oil-gas-anomaly-detection-gnn.git
cd oil-gas-anomaly-detection-gnn
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Model

### Preprocess the dataset

```bash
python src/data_processing.py
```

### Train the model

```bash
python src/training.py
```

### Evaluate performance

```bash
python src/evaluation.py
```

---

## Results

Experimental results show that the proposed framework significantly improves anomaly detection performance.

Under **time-based evaluation**:

- **ROC-AUC ≈ 0.98**
- **Anomaly Recall > 0.93**

The results demonstrate that integrating **temporal modeling with graph-based relational learning** improves robustness and detection capability in complex oil and gas production networks.

---

## Citation

If you use this work, please cite:

```bibtex
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

- Oil and gas production monitoring  
- Pipeline anomaly detection  
- Industrial IoT monitoring  
- Energy infrastructure analytics  
- Smart production optimization systems

---

## License

This repository is released for **academic and research purposes**.
