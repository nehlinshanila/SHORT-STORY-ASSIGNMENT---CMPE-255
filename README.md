# When AI Finds Patterns, Can It Explain Them?

### Explainable Deep Clustering for Time Series Data — CMPE 255 Short Story

**Student:** Shanila Nehlin  
**Course:** CMPE 255 — Data Mining, Fall 2026  
**Assignment:** Individual Short Story / Research Survey Presentation  
**Main paper:** Schlegel, U., Tavares, G. M., & Seidl, T. (2025), *Towards Explainable Deep Clustering for Time Series Data*  
**arXiv:** https://arxiv.org/abs/2507.20840

## Project overview

This repository contains materials for a literature-based overview of explainable deep clustering for time-series data. The central question is: **How can we explain why an unsupervised model groups certain sequences together?**

The review connects the 2025 Schlegel et al. survey to foundational and experimental studies, emphasizing architecture choices, explainability approaches, clustering metrics, published ablations, limitations, and possible applications. It is **not a new machine-learning training experiment** or a claim to reproduce published results.

## Main topics

1. Traditional clustering vs. deep representation learning (embeddings and autoencoders).
2. Four explanation families: attention, shapelets/prototypes, self-organizing maps, and post-hoc methods.
3. Seven representative methods covered by the 2025 survey (SOM-VAE, T-DPSOM, DeTSEC, Time2Feat, CDPS Shapelets, explainable EEG clustering, and CLAMP).
4. Published **SOM-VAE** ablation results and **Time2Feat** feature-selection / label-feedback experiments.
5. Clustering quality metrics (NMI, AMI, ARI) versus explanation quality (fidelity, compactness, stability).
6. Research limitations, opportunities, and domain-specific considerations.

## Publication and presentation links

> **Complete these links after publishing.** Do not submit placeholder URLs as finished deliverables.

- **Medium article:** `ADD_MEDIUM_ARTICLE_URL`
- **SlideShare presentation:** `ADD_SLIDESHARE_PRESENTATION_URL`
- **Recorded 10–15-minute video:** `ADD_VIDEO_URL_OR_LINK_TO_RECORDING_IN_THIS_REPOSITORY`
- **GitHub repository submission URL:** `ADD_PUBLIC_GITHUB_REPOSITORY_URL`

## Repository structure

```text
.
├── README.md
├── article/
│   └── Deep_Clustering_Research_Article_Reference.docx
├── presentation/
│   └── CMPE255_Explainable_Deep_Clustering_Presentation.pptx
├── script/
│   ├── 10_Minute_Presentation_Script.docx
│   └── 10_Minute_Presentation_Script.txt
├── figures/
│   ├── fig1_pipeline.png
│   ├── fig2_explainers.png
│   ├── fig3_som_nmi.png
│   └── fig4_time2feat.png
└── video/  (add your own recording)
```

The `article/` Word file is a research/reference working draft. The public Medium URL above should point to the actual final, student-authored published article.

## Reproducing the presentation (no code required)

1. Read the main survey and at least the SOM-VAE and Time2Feat experimental papers.
2. Open `presentation/CMPE255_Explainable_Deep_Clustering_Presentation.pptx` in PowerPoint or Google Slides.
3. Review chart captions and notes, particularly the different metrics and datasets.
4. Use `script/10_Minute_Presentation_Script.docx` to practice; personalize the critical-analysis slides.
5. Record a narrated presentation of **10–15 minutes** in Zoom, PowerPoint, or another screen recorder.
6. Add the actual video to `video/` if GitHub's file-size limits permit; for larger videos, use Git LFS or a linked hosted recording that meets your professor's requirements.
7. Publish the slides on SlideShare and your original article on Medium, then replace the placeholder links above.
8. Verify the repository can be viewed **without signing into GitHub**, and submit its URL in the class spreadsheet.

## Figures and provenance

All four figures in `figures/` are **new explanatory graphics**, prepared for the research synthesis. They are not screenshots from experimental notebooks. Figures 3–4 **redraw published numbers** and must retain their original source credits.

- `fig1_pipeline.png`: conceptual deep-clustering and explanation pipeline (synthesis from Schlegel et al. and deep clustering literature).
- `fig2_explainers.png`: original illustration of four explanation styles.
- `fig3_som_nmi.png`: published SOM-VAE / variant mean NMI values from Fortuin et al., Table 1, 16 clusters; selected MNIST/Fashion-MNIST values, average of 10 runs. These particular ablations were evaluated on image benchmarks.
- `fig4_time2feat.png`: selected hierarchical-clustering AMI values from Bonifati et al., Table 5. `T2F0` uses no labels; `T2F5` uses 50% labels per cluster.

**Important:** NMI and AMI are different measures. Results from different datasets or experimental setups should not be compared as if they were a single leaderboard.

## References

1. Schlegel, U., Tavares, G. M., & Seidl, T. (2025). *Towards Explainable Deep Clustering for Time Series Data*. arXiv:2507.20840. https://arxiv.org/abs/2507.20840
2. Xie, J., Girshick, R., & Farhadi, A. (2016). *Unsupervised Deep Embedding for Clustering Analysis*. ICML. https://proceedings.mlr.press/v48/xieb16.html
3. Zhou, S., et al. (2024 online / 2025 issue). *A Comprehensive Survey on Deep Clustering: Taxonomy, Challenges, and Future Directions*. ACM Computing Surveys. https://doi.org/10.1145/3689036
4. Ienco, D., & Interdonato, R. (2020). *Deep Multivariate Time Series Embedding Clustering via Attentive-Gated Autoencoder*. PAKDD. https://doi.org/10.1007/978-3-030-47426-3_25
5. Jain, S., & Wallace, B. C. (2019). *Attention Is Not Explanation*. NAACL. https://aclanthology.org/N19-1357/
6. Fortuin, V., et al. (2019). *SOM-VAE: Interpretable Discrete Representation Learning on Time Series*. ICLR. https://openreview.net/forum?id=rygjcsR9Y7
7. Manduchi, L., et al. (2021). *T-DPSOM: An Interpretable Clustering Method for Unsupervised Learning of Patient Health States*. ACM CHIL. https://doi.org/10.1145/3450439.3451872
8. Bonifati, A., et al. (2022). *Time2Feat: Learning Interpretable Representations for Multivariate Time Series Clustering*. PVLDB. https://doi.org/10.14778/3565816.3565822
9. El Amouri, H., et al. (2023). *Constrained DTW Preserving Shapelets for Explainable Time-Series Clustering*. Pattern Recognition. https://doi.org/10.1016/j.patcog.2023.109804
10. Ribeiro, M. T., Singh, S., & Guestrin, C. (2016). *Why Should I Trust You? Explaining the Predictions of Any Classifier*. KDD. https://doi.org/10.1145/2939672.2939778

## Notes on academic use

The primary 2025 paper is a **survey**, so numerical charts in the presentation cite the *original experimental studies* rather than attributing new results to the survey authors. Adapt the commentary to accurately represent your own reading and analysis, and follow the course rules about student-authored submissions.
