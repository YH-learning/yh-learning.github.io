---
title: "Numerical Embeddings for CTR Prediction: A Taxonomy, Unified Benchmark, and Open-Source FuxiCTR Extension"

authors:
  - me
  - Hanwei Zhu
  - Tianying Liu
  - Yulou Shu
  - Siyun Hou

date: "2026-10-31T00:00:00Z"

# Schedule page publish date (NOT publication's date).
publishDate: "2026-10-31T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article"]

# Preprints typically have no formal venue; omit `publication` until the work is accepted.

peer_reviewed: false
open_access: true

abstract: |
  Numerical embeddings map scalar features into vectors before a
  click-through rate (CTR) backbone combines the fields. To our knowledge,
  NumEmbBench is the first open benchmark dedicated to comparing numerical
  embeddings for CTR prediction. We classify 18 configurations into six
  mechanism-based families and evaluate them through one FuxiCTR interface.
  After equal-budget validation tuning, we compare frozen configurations on
  three datasets, nine backbones, and five seeds under a shared train-only
  z-score protocol. DEER has the best mean rank, but six methods lead at
  least one dataset-backbone setting. A matched native-scale test changes the
  winner in 11 of 27 settings, while paired latency measurements show that
  accuracy and inference cost need not move together. Code and per-seed
  results: https://github.com/YH-learning/NumEmbBench

summary: |
  NumEmbBench: the first open benchmark for numerical embeddings in CTR
  prediction, comparing 18 configurations across three datasets, nine
  backbones, and five seeds through a unified FuxiCTR interface.

tags:
  - Click-Through Rate Prediction
  - Numerical Embeddings
  - Recommender Systems

featured: false

hugoblox:
  ids:
    arxiv: 2611.01090

links:
  - type: code
    url: https://github.com/YH-learning/NumEmbBench
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

Preprint. Code and per-seed results are available at
[github.com/YH-learning/NumEmbBench](https://github.com/YH-learning/NumEmbBench).
