---
title: "ScalarLens: Numerical Embeddings with Stable Coordinates and Contextual Responses for CTR Prediction"

authors:
  - me
  - Tianying Liu
  - Yulou Shu
  - Yong He
  - Chuan Yuan
  - Kaibin Qiu
  - Guowei Chen
  - Jiayu Zhao
  - Siyun Hou

date: "2026-09-24T00:00:00Z"

# Schedule page publish date (NOT publication's date).
publishDate: "2026-09-24T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article"]

# Preprints typically have no formal venue; omit `publication` until the work is accepted.

peer_reviewed: false
open_access: true

abstract: |
  Numerical embeddings for click-through rate (CTR) prediction are built on a
  convenient but restrictive premise: a scalar has one representation. This
  premise conflates where a value lies with what it means for the current
  sample. On the Criteo validation split, the same numerical interval carries
  residual click evidence with opposite signs across categorical and numerical
  contexts, even after additive main effects are removed. Production pipelines
  compound this mismatch because externally normalized features require
  transformations and statistics to remain synchronized between training and
  serving. We introduce SCALARLENS, a numerical embedding that preserves what
  a value is while adapting how it should be interpreted. A monotone local
  mesh constructs a stable coordinate from the focal scalar alone; bounded
  low-rank dynamics then produce a contextual response without moving that
  coordinate or replacing categorical tokens and the CTR backbone. In a
  1,539-run primary evaluation covering 19 representations, three datasets,
  nine backbones, and three seeds, SCALARLENS ranks first in 25 of 27 settings
  on original numerical scales and second in the remaining two. A controlled
  study further recovers categorical, numerical, and mixed response mechanisms
  under context shift while the focal coordinate remains exactly invariant.
  SCALARLENS therefore recasts numerical embedding as a measurement problem:
  coordinates belong to values, while predictive responses belong to values in
  context.

summary: |
  SCALARLENS is a numerical embedding that preserves a scalar's stable
  coordinate while adapting its contextual response, ranking first in 25 of 27
  evaluation settings across three datasets and nine CTR backbones.

tags:
  - Click-Through Rate Prediction
  - Recommender Systems
  - Numerical Embeddings

featured: true

hugoblox:
  ids:
    arxiv: 2609.29182

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

Preprint.
