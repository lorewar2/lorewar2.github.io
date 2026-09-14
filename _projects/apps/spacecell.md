---
title: Spacecell
subtitle:  Clustering spatial scRNA-seq data
contributors: Minindu Weerakoon
date: 2026-09-30
image: '../images/space_cell.png'
carousels: 
  - images: 
    - image: '../images/space_cell.png'
      desc: spacecell method
order: 204
---

SpaceCell is a clustering method for spatial transcriptomics that assigns cells to spatially coherent domains by combining transcriptomic and spatial information in a staged pipeline. Where histology is available, an optional cross-attention module fuses UNI-derived morphological features with graph-attention neighbourhood features to impute a denser, higher-fidelity expression matrix. The expression is then reduced with GLM-PCA and clustered with a Gaussian mixture model, and each cluster is spatially sub-clustered to locate its contiguous domains and their centres. These centres anchor a refinement step in which cells are iteratively selected to minimise a combined negative-binomial and spatial loss, retaining only the cells most representative of each domain while leaving ambiguous cells unassigned. A weighted graph, with edge weights inverse to the negative-binomial × spatial distance and assigned cells anchored together, is then partitioned by Leiden community detection to yield the final assignment. By exploiting the complementary strengths of GLM-PCA for global separation and the negative-binomial likelihood for count-aware refinement, SpaceCell recovers anatomically meaningful spatial domains in layered tissues where adjacent regions are transcriptionally similar, demonstrated on Slide-seqV2 mouse cerebellum and 10x Visium human cortex data.

### Results




