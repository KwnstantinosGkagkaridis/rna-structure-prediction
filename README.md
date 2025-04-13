# RNA Secondary Structure Prediction using the Nussinov Algorithm

This repository implements a dynamic programming approach for predicting RNA secondary structures using the **Nussinov algorithm**, with optional handling of **pseudoknots**.

## 🧬 About

RNA molecules fold into complex structures critical for their function. The **Nussinov algorithm** predicts such structures by maximizing base pair matches. This implementation includes:

- A **standard Nussinov algorithm**.
- A **modified version** that can handle **pseudoknots** by preserving them from prior annotations.
- Visualization of structural differences between the two predictions.

---

## 📂 File Overview

- `rna_structure_prediction.py`: Main script for structure prediction and visualization.
- `vdt212_sequences.txt`: Input file containing RNA sequences and annotated dot-bracket structures (1 per line).
- `README.md`: Documentation.
