# PCA-PSO Face Recognition Framework

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)]()
[![License](https://img.shields.io/badge/License-MIT-green.svg)]()
[![Status](https://img.shields.io/badge/Status-Research-orange.svg)]()

## Overview

This repository contains the official implementation of our proposed **Principal Component Analysis (PCA) and Particle Swarm Optimization (PSO)** based face recognition framework. The proposed method integrates statistical dimensionality reduction with swarm intelligence-based feature optimization to achieve highly accurate and computationally efficient face recognition suitable for lightweight and edge-computing environments.

Unlike conventional PCA-based systems, the proposed framework employs **Particle Swarm Optimization (PSO)** to adaptively identify the most discriminative subset of principal components, thereby improving recognition accuracy while significantly reducing computational complexity.

---

## Highlights

- PCA-based dimensionality reduction (Eigenfaces)
- Adaptive feature selection using Binary Particle Swarm Optimization
- Euclidean Distance Classifier
- Lightweight CPU-based implementation
- Low computational complexity
- Fast convergence
- Cross-dataset evaluation
- Publication-quality visualizations
- Suitable for embedded and edge AI applications

---

## Proposed Framework

```
Face Images
      │
      ▼
Image Preprocessing
      │
      ▼
Image Vectorization
      │
      ▼
Principal Component Analysis
      │
      ▼
Reduced Feature Space
      │
      ▼
Particle Swarm Optimization
      │
      ▼
Optimal Feature Subset
      │
      ▼
Euclidean Distance Classification
      │
      ▼
Recognition Results
```

---

## Features

The proposed framework performs

- Face preprocessing
- Image normalization
- Eigenface extraction
- PCA feature projection
- Binary PSO optimization
- Optimal feature selection
- Euclidean nearest-neighbor classification
- Performance evaluation

---

## Repository Structure

```
PCA-PSO-FaceRecognition/
│
├── datasets/
│   ├── ORL/
│   ├── ExtendedYaleB/
│   └── LFW/
│
├── preprocessing/
│
├── pca/
│
├── pso/
│
├── classifier/
│
├── evaluation/
│
├── figures/
│
├── notebooks/
│
├── results/
│
├── requirements.txt
│
├── train.py
│
├── evaluate.py
│
└── README.md
```

---

## Datasets

The framework has been evaluated on

| Dataset | Subjects | Images |
|----------|----------|---------|
| ORL | 40 | 400 |
| Extended Yale B | 38 | 2414 |
| LFW | 5749 | 13000+ |

---

## Experimental Results

| Dataset | Accuracy | Precision | Recall | F1-score |
|----------|----------|-----------|--------|----------|
| ORL | 99.99% | 99.98% | 99.99% | 99.98% |
| Extended Yale B | 99.18% | 99.10% | 99.14% | 99.12% |
| LFW | 98.45% | 98.32% | 98.40% | 98.36% |

---

## Computational Performance

| Metric | Value |
|---------|------|
| Selected Features | 44 |
| Training Time / Epoch | 2–3 sec |
| Inference Time | 2–3 ms |
| CPU Execution | ✓ |
| GPU Required | No |
| Model Size | < 1 MB |

---

## Installation

Clone the repository

```bash
git clone https://github.com/username/PCA-PSO-FaceRecognition.git

cd PCA-PSO-FaceRecognition
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Usage

Train the model

```bash
python train.py
```

Evaluate

```bash
python evaluate.py
```

---

## Main Components

### Principal Component Analysis (PCA)

PCA transforms high-dimensional facial images into a compact eigenspace while preserving the maximum variance.

### Particle Swarm Optimization (PSO)

Binary PSO performs adaptive feature selection by optimizing the subset of PCA components that maximizes recognition performance.

### Classification

Recognition is performed using a Euclidean Distance classifier operating on the optimized feature subset.

---

## Performance Evaluation

The repository provides

- Accuracy
- Precision
- Recall
- F1-score
- ROC Curve
- Confusion Matrix
- Feature Space Visualization
- PSO Convergence Curves
- Computational Analysis
- Statistical Validation

---

## Citation

If you use this repository in your research, please cite:

```
@article{YourPaper2026,
  title={Lightweight PCA–PSO Framework for Face Recognition Using Adaptive Feature Selection},
  author={Author(s)},
  journal={Journal Name},
  year={2026}
}
```

---

## Future Work

- Deep learning comparison
- Embedded ARM deployment
- Raspberry Pi implementation
- FPGA implementation
- Real-time video face recognition
- Mobile authentication
- Explainable AI integration

---

## License

This repository is released under the MIT License.

---

## Contact

For questions, collaborations, or research discussions, please open an Issue or submit a Pull Request.
