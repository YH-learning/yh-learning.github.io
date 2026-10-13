---
title: "PRIME: Mitigating Subgroup Optimization Competition in Shared CTR Top Networks with Plug-in Residual Input-Conditioned Mixture of Expert"

authors:
  - me
  - Siyun Hou
  - Tianying Liu
  - Yulou Shu
  - Yong He
  - Chuan Yuan
  - Kaibin Qiu
  - Guowei Chen
  - Jiayu Zhao
  - Chao Yu
  - Ke Ding

date: "2026-08-31T00:00:00Z"

# Schedule page publish date (NOT publication's date).
publishDate: "2026-08-31T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article"]

# Preprints typically have no formal venue; omit `publication` until the work is accepted.

peer_reviewed: false
open_access: true

abstract: |
  Click-through rate (CTR) models vary in feature-interaction design, yet their
  top networks usually remain a single multilayer perceptron shared by all
  examples. Heterogeneous user, item, and context subgroups therefore update
  the same parameters; weakly aligned learning signals make the aggregate
  gradient a compromise among competing directions. We study the competition
  on Avazu with 4 models and 4 semantic fields. Across all architectures,
  semantic subgroups show lower Top-NN gradient cosine similarity than random
  groups matched by sample size and label ratio, with reductions of
  0.23-0.37. This competition motivates input-conditioned experts, but
  directly replacing an established Dense mapping changes its initial
  function, sharing pattern, and capacity, obscuring the source of gains. We
  introduce PRIME (Plug-in Residual Input-conditioned Mixture of Experts), a
  Dense-anchored mixture of low-rank residual experts. PRIME anchors the
  original prediction and uses zero-residual initialization to match the
  Dense baseline exactly at training onset. Input-dependent routing weights
  low-rank experts for example-specific logit corrections; multi-bag
  aggregation and EMA load biases stabilize conditional estimation. We
  evaluate PRIME on held-out Avazu and Criteo test sets across 13 CTR
  architectures and five paired seeds. Median paired AUC gains are +0.0022 and
  +0.0066, with LogLoss reductions of 0.0011 and 0.0081, respectively. On
  FiBiNET and DCNv2, PRIME outperforms APG in all ten seed-level AUC
  comparisons while using fewer parameters and lower inference latency on both
  backbones.

summary: |
  PRIME is a Dense-anchored mixture of low-rank residual experts that adds
  input-dependent capacity to shared CTR top networks while preserving the
  Dense path and its optimization stability, improving median paired AUC on
  Avazu and Criteo across 13 CTR architectures.

tags:
  - Click-Through Rate Prediction
  - Recommender Systems
  - Mixture of Experts

featured: true

hugoblox:
  ids:
    arxiv: 2608.30449

links:
  - type: code
    url: https://github.com/YH-learning/PRIME
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

Preprint. Code is available at
[github.com/YH-learning/PRIME](https://github.com/YH-learning/PRIME).
