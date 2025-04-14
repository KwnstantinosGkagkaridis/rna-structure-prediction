# RNA Secondary Structure Prediction using Nussinov Algorithm

This repository contains a Python implementation of algorithms for predicting RNA secondary structures, including the standard Nussinov algorithm and a modified version that accounts for pseudoknots. The algorithms utilize dynamic programming to maximize complementary base pairs in RNA sequences.

## Overview

RNA folding is a critical biological process that determines its structure and function. This project implements:
1. **Standard Nussinov Algorithm**: Predicts RNA secondary structures without considering pseudoknots.
2. **Modified Nussinov Algorithm**: Incorporates pseudoknots into the folding predictions by blocking specific regions during computation.

Additionally, the repository provides tools for comparing the predicted structures and visualizing differences in structure prediction results.

---

## Features

- **Standard Nussinov Algorithm**:
  - Predicts secondary RNA structure by maximizing the number of canonical base pairs (A-U, G-C, wobble G-U).
  - Uses dynamic programming to compute a scoring matrix and reconstructs the structure using backtracking.

- **Modified Nussinov Algorithm**:
  - Extends the standard algorithm to account for pseudoknots.
  - Detects pseudoknot regions in RNA sequences and prevents base pairing within these regions.
  - Incorporates both blocked regions and predicted base pairs into the final dot-bracket representation.

- **Comparison and Visualization**:
  - Computes symmetric differences between standard and pseudoknot-aware structures.
  - Visualizes the pairwise distance (structure discrepancy) as a function of RNA sequence length.

---

## Algorithms

### **1. Standard Nussinov Algorithm**
- **Goal**: Maximize the number of base pairs that form valid bonds.
- **Steps**:
  1. Build a scoring matrix where each entry represents the maximum number of pairs for subsequences.
  2. Use base-pairing rules to determine valid pairs: A-U, G-C, and wobble G-U.
  3. Use dynamic programming to fill the matrix by considering:
     - Left cell
     - Down cell
     - Diagonal cell (valid pairs)
  4. Reconstruct the optimal structure using backtracking.
- **Output**: RNA structure in dot-bracket notation.

### **2. Modified Nussinov Algorithm (with Pseudoknots)**
- **Goal**: Extend predictions to handle pseudoknots by blocking certain base-pairing regions.
- **Steps**:
  1. Detect pseudoknot regions from an input structure.
  2. Divide the sequence into regions (blocked and unblocked).
  3. Apply the standard Nussinov algorithm separately to each region.
  4. Combine blocked regions and predicted base pairs into the final dot-bracket structure.
- **Output**: RNA structure with pseudoknots in dot-bracket notation.

---

## Visualization

The repository generates a scatter plot showing:
- X-axis: RNA sequence length.
- Y-axis: Pairwise distance (symmetric difference) between structures predicted by the standard and pseudoknot-aware algorithms.
