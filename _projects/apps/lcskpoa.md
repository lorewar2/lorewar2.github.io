---
title: LCSkPOA
subtitle: Enabling banded semi-global partial order alignments via efficient and accurate backbone generation through extended LCSk++
contributors: Minindu Weerakoon
date: 2025-05-30
image: '../images/lcskpoa.png'
carousels: 
  - images: 
    - image: '../images/lcskpoa.png'
      desc: lcskpoa method
order: 201
---

Abstract

Background

Most multiple sequence alignment and string-graph alignment algorithms focus on global alignment, but many applications exist for semi-global and local string-graph alignment. Long reads require enormous amounts of memory and runtime to fill out large dynamic programming tables. Effective algorithms for finding the backbone and thus defining a band of an alignment such as the longest common subsequence with kmer matches (LCSk++) exist but do not work with graphs. This study introduces an adaptation of the Longest Common Subsequence with kmer matches (LCSk++) algorithm tailored for graph structures, particularly focusing on Partial Order Alignment (POA) graphs. POA graphs, which are directed acyclic graphs, represent multiple sequence alignments and effectively capture the relationships between sequences. State-of-the-art methods like ABPOA and SPOA improve upon POA, while ABPOA incorporates banding, SPOA does not; however, neither utilizes parallel processing despite leveraging SIMD for faster matrix calculations. Our approach addresses these limitations by extending the LCSk++ algorithm to handle the complexities of graph-based alignment while incorporating SIMD, banding, and parallel processing for enhanced efficiency.

Results

Our extended LCSk++ algorithm integrates dynamic programming and graph traversal techniques to detect conserved regions within POA graphs, termed the LCSk++ backbone. This backbone enables precise banding of the POA matrix for all alignment modes (global, semi-global, and local). Unlike ABPOA, which only allows banded global alignment, our approach enables broader flexibility and significantly improves consensus sequence construction. While supporting more alignment modes than ABPOA, it also outperforms SPOA’s global alignment, with substantial memory savings (up to 98%) and significant run-time reductions (up to 25x), particularly for long sequences (> 30,000 bp). Our method maintains high alignment accuracy and proves effective across various string lengths and datasets, including synthetic and PacBio HiFi reads. Parallel processing further enhances runtime efficiency, achieving up to 150x speed improvements on conventional PCs.

Conclusion

The extended LCSk++ algorithm for graph structures offers a substantial advancement in sequence alignment technology. It effectively reduces memory consumption and optimizes run times without compromising alignment quality, thus providing a robust solution for all alignment modes (global, local, and semi-global) in POA. This method enhances the utility of POA in critical applications such as multiple sequence alignment for phylogeny construction and graph-based reference alignment.

### Results

https://link.springer.com/article/10.1186/s12859-025-06293-z


