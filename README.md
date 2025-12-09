# Comparative Structure of Real-World Ecological Networks  
### Wild Bird Social Network & Scotch Broom Interaction Web

[![Python](https://img.shields.io/badge/Python-3.10-blue.svg)]()
[![NetworkX](https://img.shields.io/badge/NetworkX-Analysis-orange.svg)]()
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Figures-green.svg)]()
[![Reproducible](https://img.shields.io/badge/Reproducible-Yes-success.svg)]()

This repository contains the full analytical workflow, Python code, figures, and metric tables for a comparative network analysis of two biological systems:

- **Wild Bird Social Network** :RFID-based co-occurrence interactions among *Parus major*.  
- **Scotch Broom Interaction Web**: Multi-trophic ecological network centered on *Cytisus scoparius*.

The project examines structure, motifs, community organization, centrality, null models, and robustness to perturbations through a unified graph-theoretic framework.

---

## 📌 Project Objectives

- Represent each dataset as an undirected graph.
- Compute and compare:
  - Spectral partitions and eigenstructure  
  - Clustering, triangles, and four-cycles  
  - Erdős–Rényi (ER) and configuration-model (CM) null expectations  
  - Louvain community modularity  
  - Degree, closeness, and betweenness centrality  
  - Robustness curves (random, degree-based, betweenness-based removal)
- Identify structural similarities across ecological and behavioral systems.

---



## 📊 Key Results (Summary)

### **Structural Metrics**
| Metric | Wildbird | Scotch |
|-------|----------|--------|
| Nodes | 169 | 154 |
| Edges | 2758 | 366 |
| Clustering (real) | 0.77 | 0.14 |
| Modularity | 0.37 | 0.53 |
| Louvain communities | 5 | 7 |
| Triangles (real) | 27,886 | 358 |
| 4-cycles (real) | 961,915 | 5,368 |

### **Robustness (AUC values)**  
| Strategy | Wildbird | Scotch |
|----------|----------|--------|
| Random | 0.48 | 0.37 |
| Degree-targeted | 0.38 | 0.09 |
| Betweenness-targeted | 0.25 | 0.07 |

### **Interpretation**
- Wildbird network: dense, highly clustered, strong redundancy.  
- Scotch broom web: modular, trophically structured, more fragile under targeted attacks.  
- Both networks deviate strongly from ER and CM null models → non-random architecture.

---
## 👥 Team Contributions

| Team Member      | Contribution Description |
|------------------|---------------------------|
| **Isaac O. A.**  | Lead analysis, methodology design, Python scripting, and primary report writing. |
| **Michael G.**   | Data curation, figure preparation, development of null-model simulations, and proofreading. |
| **Bridget D.**   | Statistical comparison, literature review, ecological interpretation, link prediction,and proofreading. |
---

## 🧾 Citation

If you use this repository, please cite:

**Amanor, I. O., Gleyzer, M., & Donohue, B. (2025).  
*Comparative Structure of Real-World Ecological Networks: Wild Bird Social Network and Scotch Broom Interaction Web*.**

---

## 🙏 Acknowledgments  

We acknowledge **Professor Chenyu** for supervising the project and  
**Professor Philip Knight (AIMS South Africa, University of Strathclyde)**  
for providing access to key datasets and guidance that made this study possible.

