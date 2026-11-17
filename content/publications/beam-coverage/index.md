---
title: "Where Beam Search Loses Top-Ranked Items: First-Step Coverage in Generative Recommendation"

authors:
  - me
  - Hanwei Zhu

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
  Generative recommendation can reproduce a wider beam's ranked output with
  roughly half the prefix-capacity budget by reallocating retention capacity
  across semantic-ID positions. We identify a first-step coverage bottleneck:
  across six full-test settings of the TIGER generative recommender spanning
  three domains and two identifier constructions, every pruned exact top-10
  path is first lost at the initial decoding step. An exact-catalog reference
  isolates search losses and guides a controlled budget intervention. Moving
  width to the first step raises Search Recall@10 by 0.96-10.90 percentage
  points at Beam-50's unchanged budget. Across all 77,373 test users with
  residual-quantized variational autoencoder (RQ-VAE) tokenization, the
  reallocated schedule reproduces Beam-100's ordered top-10 at nominal budgets
  of 151 rather than 301, without retraining or changing identifiers or
  scores. Matched-output timing saves 6.35-6.39% of decoder latency; profiling
  identifies the execution costs that limit the translation from reduced
  search work to runtime savings. Larger-candidate experiments reveal how
  output size changes retention requirements. These findings make budget
  placement an actionable serving decision: locate ranking loss, redirect
  search capacity, and preserve downstream inputs before increasing uniform
  beam width.

summary: |
  Reallocating beam-search capacity to the first decoding step reproduces
  Beam-100's ordered top-10 at roughly half the prefix budget (151 vs. 301) in
  TIGER-style generative recommendation, without retraining.

tags:
  - Generative Recommendation
  - Recommender Systems

featured: false

hugoblox:
  ids:
    arxiv: 2611.01072

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
