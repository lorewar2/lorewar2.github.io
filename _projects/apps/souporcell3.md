---
title: souporcell3
subtitle:  robust demultiplexing for high-donor single-cell RNA-seq datasets
contributors: Minindu Weerakoon
date: 2026-05-30
image: '../images/souporcell3.png'
carousels: 
  - images: 
    - image: '../images/souporcell3.png'
      desc: souporcell3 method
order: 202
---

Motivation

Accurate demultiplexing of pooled single-cell RNA-seq (scRNA-seq) data is critical for large-scale studies. However, existing methods like vireo, while effective up to ∼16 donors, often struggle with poor clustering due to local optima as donor numbers rise. In high-donor scenarios, overlapping genotypes, a dense genotype space, and increased doublet formation make demultiplexing challenging, requiring methods that are robust to sparse, high-dimensional data and maintain reliable accuracy even as sample complexity grows.

Results

We present an enhanced version of souporcell capable of demultiplexing up to 64 donors. The method uses 10× merge for initialization, K-Harmonic Means for robust clustering, and iterative refinement with reinitialization of low-quality clusters and locking of high-quality ones. Compared to vireo, overclustered vireo, and the original souporcell, our approach completely eliminates incorrectly merged clusters and achieves consistently high Adjusted Rand Index (ARI) scores across various doublet rates, demonstrating improved accuracy and scalability.
Availability and implementation

Souporcell3 is freely available under the MIT open-source license at https://github.com/wheaton5/souporcell.

### Results

https://academic.oup.com/bioinformatics/article/42/3/btag117/8513494


