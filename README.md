# Recommendation System

---

Implementation of a recommendation system built from scratch using **Non-negative Matrix Factorization (NMF)** and **Min-Hash**, achieving **85%+ accuracy** on both validation and test data.

---

## Problem Description

A binary recommendation task: predict whether a user will like (1) or dislike (0) an item, given a highly sparse user-item interaction matrix.

**Dataset characteristics:**
- **Sparsity:** ~99.4% — most user-item pairs are unrated
- **Class imbalance:** 82% dislikes, 18% likes (ratio ~1:0.21)
- **User activity:** average 17 ratings per user (14 dislikes, 3 likes)

---

## Algorithms

### Non-negative Matrix Factorization (NMF)
Decomposes the sparse user-item matrix into atrices, capturing latent factors thatrepresent user preferences and item characteristics.

### Min-Hash
A locality-sensitive hashing technique used arity between users or items, enabling fastapproximate nearest-neighbour lookups in sparse data.

---

## Results

| Model | Validation Accuracy | Test Accuracy |
|-------|-------------------|---------------
| NMF | 85%+ | 85%+ |
| Min-Hash | 85%+ | 85%+ |

---

## Dataset

| File | Description |
|------|-------------|
| `train_data_2026.npy` | Training user-item
| `val_data_2026.npy` | Validation set |
| `test_data_2026.npy` | Test set |

Data format: binary ratings matrix where `1` = unrated.

---

## Constraints

Built using only **NumPy, SciPy, Matplotlib,ing frameworks.

---

## Setup

```bash
pip install numpy scipy matplotlib pandas
jupyter notebook dm_2026_lab_assignment_2_pi

```
