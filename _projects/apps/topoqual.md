---
title: Topoqual
subtitle: HiFi longread consensus error correction and quality score prediction tool
contributors: Minindu Weerakoon
date: 2025-01-30
image: '../images/topoqual.png'
carousels: 
  - images: 
    - image: '../images/topoqual.png'
      desc: topoqual method
order: 200
---

Abstract

Background

Pacific Biosciences (PacBio) circular consensus sequencing (CCS), also known as high fidelity (HiFi) technology, has revolutionized modern genomics by producing long (10 + kb) and highly accurate reads. This is achieved by sequencing circularized DNA molecules multiple times and combining them into a consensus sequence. Currently, the accuracy and quality value estimation provided by HiFi technology are more than sufficient for applications such as genome assembly and germline variant calling. However, there are limitations in the accuracy of the estimated quality scores when it comes to somatic variant calling on single reads.

Results

To address the challenge of inaccurate quality scores for somatic variant calling, we introduce TopoQual, a novel tool designed to enhance the accuracy of base quality predictions. TopoQual leverages techniques including partial order alignments (POA), topologically parallel bases, and deep learning algorithms to polish consensus sequences. Our results demonstrate that TopoQual corrects approximately 31.9% of errors in PacBio consensus sequences. Additionally, it validates base qualities up to q59, which corresponds to one error in 0.9 million bases. These improvements will significantly enhance the reliability of somatic variant calling using HiFi data.

Conclusion

TopoQual represents a significant advancement in genomics by improving the accuracy of base quality predictions for PacBio HiFi sequencing data. By correcting a substantial proportion of errors and achieving high base quality validation, TopoQual enables confident and accurate somatic variant calling. This tool not only addresses a critical limitation of current HiFi technology but also opens new possibilities for precise genomic analysis in various research and clinical applications.

### Results

https://link.springer.com/article/10.1186/s12859-024-06020-0


