---
title: "IV-CoT: Implicit Visual Chain-of-Thought for Structure-Aware Text-to-Image Generation"

authors:
  - Zixuan Li
  - Haokun Lin
  - Yicheng Xiao
  - Zhiwei Li
  - Xinyang Song
  - Zelong Zheng
  - Yong He
  - me
  - Ke Ding
  - Chao Yu
  - Chuan Yuan
  - Qi Li
  - Zhenan Sun

date: "2026-06-23T00:00:00Z"

# Schedule page publish date (NOT publication's date).
publishDate: "2026-06-23T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article"]

# Preprints typically have no formal venue; omit `publication` until the work is accepted.

peer_reviewed: false
open_access: true

abstract: |
  Unified multi-modal large language models (MLLMs) have achieved strong
  text-to-image generation quality, but still struggle with structure-aware
  prompt following, where object counts, spatial relations, attribute
  bindings, and coarse layouts must be preserved. We attribute this limitation
  in part to the entanglement of structural planning and appearance rendering
  within a single conditioning stream. To address this issue, we propose
  Implicit Visual Chain-of-Thought (IV-CoT), a latent visual reasoning
  framework for query-conditioned image generation. IV-CoT decomposes the
  visual conditioning queries into a structural-to-semantic cascade, where
  structural queries first form a latent visual plan and semantic queries then
  render appearance conditioned on this plan. To guide the structural queries,
  we introduce training-only sketch supervision, which encourages them to
  capture structure from sketches without requiring sketch extraction or
  intermediate decoding at inference time. IV-CoT performs implicit CoT
  reasoning in a single forward pass and achieves superior results on GenEval
  and T2I-CompBench.

summary: |
  IV-CoT is a latent visual reasoning framework that decomposes visual
  conditioning queries into a structural-to-semantic cascade, improving
  structure-aware text-to-image generation on GenEval and T2I-CompBench.

tags:
  - Text-to-Image Generation
  - Multi-modal Large Language Models
  - Visual Chain-of-Thought

featured: false

hugoblox:
  ids:
    arxiv: 2606.24849

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
