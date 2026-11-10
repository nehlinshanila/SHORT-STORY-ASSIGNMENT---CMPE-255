# When AI Groups Time Series, Can It Explain Why?

**CMPE 255 — Data Mining | Short Story Assignment**

**Author:** Shanila Nehlin  
**Topic:** Explainable Deep Clustering for Time Series Data

## Project Overview

Deep learning can discover meaningful patterns in time-series data, but an important challenge remains: **Can AI explain why certain time series belong to the same cluster?**

This project explores explainable deep clustering, focusing on methods that combine unsupervised learning with interpretable results.

The primary research paper is *Towards Explainable Deep Clustering for Time Series Data* by Udo Schlegel, Gabriel Marques Tavares, and Thomas Seidl (2025), accepted at the TempXAI Workshop at ECML-PKDD 2025.

**Research Paper:** https://arxiv.org/pdf/2507.20840

## Project Deliverables

| Deliverable | Link |
|---|---|
| Medium Article | [When AI Groups Time Series, Can It Explain Why?](https://medium.com/@nehlinshanila/when-ai-groups-time-series-can-it-explain-why-b1ed1d23a4c6) |
| PowerPoint Presentation | (https://github.com/nehlinshanila/SHORT-STORY-ASSIGNMENT---CMPE-255/blob/master/CMPE255_Presentation.pptx) |
| Video Presentation (10–15 minutes) | (https://youtu.be/PvW0Em6Yzk8) |

## Key Topics Covered

### 1. Understanding Time-Series Clustering

Time-series clustering groups sequences based on similarities in temporal patterns. Applications include healthcare monitoring, financial analysis, industrial sensors, and human activity recognition.

### 2. Deep Clustering Architecture

A typical deep clustering system uses:

- Time-series input
- Deep neural network encoder
- Latent feature representations
- Clustering algorithm
- Explainability mechanisms

### 3. Explainability Techniques

The research investigates several approaches:

- Attention mechanisms
- Shapelet-based explanations
- Self-organizing maps (SOM)
- Prototype-based representations
- Post-hoc interpretability

### 4. Research Comparison

The project reviews important methods, including:

- **DeTSEC:** Attentive gated deep clustering for multivariate time series.
- **Time2Feat:** Interpretable feature extraction and selection.
- **SOM-VAE:** Self-organizing maps with deep representation learning.
- **T-DPSOM:** Interpretable clustering of temporal patient health states.
- **Shapelet-based approaches:** Explanations based on recognizable subsequences.

### 5. Evaluation Metrics

Clustering quality is discussed using:

- Normalized Mutual Information (NMI)
- Adjusted Mutual Information (AMI)
- Adjusted Rand Index (ARI)

Explanation quality is considered separately through faithfulness, stability, and human interpretability.

### 6. Ablation Studies

The project discusses experiments from the original research papers that examine how individual components, such as attention gating, bidirectional sequence modeling, and feature selection, contribute to performance.

## Key Findings and Personal Analysis

My main observation is that achieving high clustering accuracy does not necessarily make a model explainable.

Although deep learning can identify complex relationships within time-series data, its internal representations often remain difficult for humans to understand.

Attention mechanisms, interpretable features, shapelets, and prototype representations provide promising approaches to address this challenge.

However, visual explanations alone are insufficient. Future research should also evaluate whether those explanations faithfully reflect the model's behavior.

**My conclusion:** Explainable deep clustering should optimize not only clustering quality but also the reliability and usefulness of the explanations it produces.

## Repository Structure

The repository contains the following project materials:

- `README.md` — Project documentation
- `article/` — Original Medium article and document
- `figures/` — Research diagrams and visualizations
- `slides/` — PowerPoint and PDF presentation
- `video/` — Presentation narration script and recorded video
- `references/` — Research citations and source attribution
- `scripts/` — Scripts for generating diagrams and slides

## Research Integrity

The main 2025 paper is a survey. Numerical results and ablation findings discussed in this project come from the original cited studies.

The figures are primarily original explanatory illustrations, with published results clearly attributed. This project does not claim to have independently trained or benchmarked the surveyed deep clustering models.

## References

1. Schlegel, U., Tavares, G. M., & Seidl, T. (2025). *Towards Explainable Deep Clustering for Time Series Data*. https://arxiv.org/abs/2507.20840

2. Ienco, D., & Interdonato, R. (2020). *Deep Multivariate Time Series Embedding Clustering via Attentive-Gated Autoencoder*. https://pmc.ncbi.nlm.nih.gov/articles/PMC7206254/

3. Bonifati, A., et al. (2022). *Time2Feat: Learning Interpretable Representations for Multivariate Time Series Clustering*. https://www.vldb.org/pvldb/vol16/p193-tiano.pdf

4. Fortuin, V., et al. (2019). *SOM-VAE: Interpretable Discrete Representation Learning on Time Series*. https://arxiv.org/abs/1806.02199

5. Manduchi, L., et al. (2021). *T-DPSOM: An Interpretable Clustering Method for Unsupervised Learning of Patient Health States*. https://doi.org/10.1145/3450439.3451872


---

**Course:** CMPE 255 — Data Mining  
**Institution:** San José State University  
**Author:** Shanila Nehlin
