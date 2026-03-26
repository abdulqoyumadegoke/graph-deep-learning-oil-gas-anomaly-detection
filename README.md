Graph-Based Deep Learning for Anomaly Detection in Oil & Gas Production Networks

This repository contains the implementation of the research paper:

"Graph-Based Deep Learning for Intelligent Detection of Energy Losses, Theft, and Operational Inefficiencies in Oil & Gas Production Networks."

The paper is available on arXiv:
https://arxiv.org/abs/2603.14406

Overview

Energy losses, production theft, and operational inefficiencies remain persistent challenges in oil and gas production systems due to complex interdependencies among wells, facilities, and surface infrastructure.

This project introduces a spatiotemporal graph-based deep learning framework capable of detecting anomalies across production networks by capturing both:

Temporal dynamics of production variables
Relational dependencies among wells and facilities

The framework models production systems as hierarchical graphs and leverages Temporal Graph Attention Networks (TGAT) to detect abnormal behavior patterns.

Key Features
Spatiotemporal graph modeling of production systems
Weakly supervised anomaly labeling using physical heuristics
Temporal Graph Attention Network for relational learning
Robust evaluation using both random and time-based splits
High anomaly detection performance under non-stationary conditions
Model Architecture

The proposed framework integrates:

Production Data Processing
Graph Construction (Wells–Facilities–Field Hierarchy)
Temporal Sequence Modeling
Graph Attention Learning
Anomaly Classification
Performance

Experimental evaluation shows strong performance:

Metric	Score
ROC-AUC	~0.98
Anomaly Recall	>0.93

The model significantly outperforms:

Traditional Machine Learning models
Sequence-only deep learning approaches
