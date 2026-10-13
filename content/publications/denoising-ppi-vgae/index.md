---
title: "Denoising Protein-Protein Interaction Network via Variational Graph Auto-Encoder for Protein Complex Detection"

authors:
  - me
  - Jihong Guan
  - Tianying Liu

date: "2020-06-01T00:00:00Z"

# Schedule page publish date (NOT publication's date).
publishDate: "2020-06-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication metadata — structured fields used by citation styles and BibTeX export.
publication:
  name: "Journal of Bioinformatics and Computational Biology"
  short_name: "JBCB"
  volume: 18
  issue: 3
  pages: "2040010"

peer_reviewed: true
open_access: false

abstract: |
  Identifying protein complexes is an important issue in computational
  biology, as it benefits the understanding of cellular functions and the
  design of drugs. In the past decades, many computational methods have been
  proposed by mining dense subgraphs in Protein-Protein Interaction Networks
  (PINs). However, the high rate of false positive/negative interactions in
  PINs prevents accurately detecting complexes directly from the raw PINs. In
  this paper, we propose a denoising approach for protein complex detection by
  using variational graph auto-encoder. First, we embed a PIN to vector space
  by a stacked graph convolutional network (GCN), then decide which
  interactions in the PIN are credible. If the probability of an interaction
  being credible is less than a threshold, we delete the interaction. In such
  a way, we reconstruct a reliable PIN. Following that, we detect protein
  complexes in the reconstructed PIN by using several typical detection
  methods, including CPM, Coach, DPClus, GraphEntropy, IPCA and MCODE, and
  compare the results with those obtained directly from the original PIN. We
  conduct the empirical evaluation on four yeast PPI datasets (Gavin, Krogan,
  DIP and Wiphi) and two human PPI datasets (Reactome and Reactomekb),
  against two yeast complex benchmarks (CYC2008 and MIPS) and three human
  complex benchmarks (REACT, REACT_uniprotkb and CORE_COMPLEX_human),
  respectively. Experimental results show that with the reconstructed PINs
  obtained by our denoising approach, complex detection performance can get
  obviously boosted, in most cases by over 5%, sometimes even by 200%.
  Furthermore, we compare our approach with two existing denoising methods
  (RWS and RedNemo) while varying different matching rates on separate complex
  distributions. Our results show that in most cases (over 2/3), the proposed
  approach outperforms the existing methods.

summary: |
  A variational graph auto-encoder based denoising approach that reconstructs
  reliable protein-protein interaction networks, boosting protein complex
  detection performance by over 5% and sometimes even by 200%.

tags:
  - Protein Complex Detection
  - Variational Graph Auto-Encoder
  - Bioinformatics

featured: false

hugoblox:
  ids:
    doi: 10.1142/S0219720020400107

links:
  - type: code
    url: ""
  - type: dataset
    url: ""
  - type: poster
    url: ""
  - type: project
    url: ""
  - type: slides
    url: ""
  - type: source
    url: ""
  - type: video
    url: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
projects: []

# Slides (optional).
slides: ""
---

> [!NOTE]
> Click the *Cite* button above to import the publication metadata into your
> reference management software.

Published in *Journal of Bioinformatics and Computational Biology*, vol. 18,
no. 3, 2040010, 2020.
DOI: [10.1142/S0219720020400107](https://doi.org/10.1142/S0219720020400107).
