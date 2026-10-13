---
title: "Accurately Detecting Protein Complexes by Graph Embedding and Combining Functions with Interactions"

authors:
  - me
  - Yunjia Shi
  - Jihong Guan
  - Shuigeng Zhou

date: "2020-05-01T00:00:00Z"

# Schedule page publish date (NOT publication's date).
publishDate: "2020-05-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication metadata — structured fields used by citation styles and BibTeX export.
publication:
  name: "IEEE/ACM Transactions on Computational Biology and Bioinformatics"
  short_name: "IEEE/ACM TCBB"
  volume: 17
  issue: 3
  pages: "777-787"

peer_reviewed: true
open_access: false

abstract: |
  Identifying protein complexes is helpful for understanding cellular
  functions and designing drugs. In the last decades, many computational
  methods have been proposed based on detecting dense subgraphs or
  subnetworks in Protein-Protein Interaction Networks (PINs). However, the
  high rate of false positive/negative interactions in PINs prevents from the
  achievement of satisfactory detection results directly from PINs, because
  most of such existing methods exploit mainly topological information to do
  network partitioning. In this paper, we propose a new approach to protein
  complex detection by merging topological information of PINs and functional
  information of proteins. We first split proteins to a number of protein
  groups from the perspective of protein functions by using FunCat data. Then,
  for each of the resulting protein groups, we calculate two protein-protein
  similarity matrices: one is computed by using graph embedding over a PIN,
  the other is by using GO terms, and combine these two matrices to get an
  integrated similarity matrix. Following that, we cluster the proteins in
  each group based on the corresponding integrated similarity matrix, and
  obtain a number of small protein clusters. We map these clusters of proteins
  onto the PIN, and get a number of connected subgraphs. After a round of
  merging of overlapping subgraphs, finally we get the detected complexes. We
  conduct empirical evaluation on four PPI datasets (Collins, Gavin, Krogan,
  and Wiphi) with two complex benchmarks (CYC2008 and MIPS). Experimental
  results show that our method performs better than the state-of-the-art
  methods.

summary: |
  A protein complex detection approach that merges graph embedding over PPI
  networks with GO-term functional information, outperforming state-of-the-art
  methods on four PPI datasets and two complex benchmarks.

tags:
  - Protein Complex Detection
  - Graph Embedding
  - Bioinformatics

featured: false

hugoblox:
  ids:
    doi: 10.1109/TCBB.2019.2897769

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

Published in *IEEE/ACM Transactions on Computational Biology and
Bioinformatics*, vol. 17, no. 3, pp. 777-787, 2020.
DOI: [10.1109/TCBB.2019.2897769](https://doi.org/10.1109/TCBB.2019.2897769).
