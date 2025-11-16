# A Hybrid Clustering--Validation Framework Using OPTICS and Multi-Algorithm Cross-Validation

This repository contains the official implementation of the hybrid
clustering--validation framework proposed in our ISI manuscript. The
framework integrates density-based clustering (OPTICS) with
multi-algorithm cross-validation to evaluate cluster stability,
structural coherence, and feature--space consistency across datasets.

## 1. Overview

Our method introduces a hybrid cross-validation strategy combining
OPTICS and four clustering algorithms to compute multi-perspective
validation metrics.

## 2. Project Structure

Azodi/ │ ├── 4algoCV.py ├── HybridCV.py ├── optics.py ├── datasets/ ├──
clustering_cv_accuracy_results.xlsx ├── optics_cv_accuracy_results.xlsx
└── README.md

## 3. Methods

### 3.1 OPTICS Clustering Module

Implements OPTICS reachability computation and density-based extraction.

### 3.2 Multi-Algorithm Cross-Validation

Includes K-Means, Agglomerative, Spectral, and GMM clustering.

### 3.3 Hybrid Metric

f1(x)= Σ (1/\|Ck\| Σ \|\|zi -- μk\|\|² )

## 4. How to Run

pip install -r requirements.txt\
python optics.py\
python 4algoCV.py\
python HybridCV.py

## 5. Reproducibility

Place datasets in datasets/ and execute HybridCV.py.

## 6. Citation

\[Authors\], "\[Article Title\]," \[Journal\], \[Year\].

## 7. License

Academic use only.
