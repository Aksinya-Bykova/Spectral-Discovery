# Spectral Discovery

A research proposal on global graph structure in recommendation systems.

## Overview

I critically analyzed **ContextGNN: Beyond Two-Tower Recommendation
Systems (ICLR 2025)** and identified a limitation in its global
representation: the global tower relies on shallow item embeddings and
does not explicitly encode the global structure of the interaction graph.

I proposed **Spectral Discovery**, an alternative approach that constructs
a spectral representation of the historical interaction graph offline
and uses its low-frequency components as a structural prior for
exploratory recommendation.

> **In short:** I took a recent ICLR 2025 architecture, identified a
> concrete limitation, and developed a testable alternative rather than
> simply reproducing the original method.

## What the proposal contains

- Critical analysis of the ContextGNN architecture and its design trade-offs
- A spectral representation based on the normalized graph Laplacian
- Low-frequency spectral coordinates as global structural representations
- Spectral clustering and latent structural archetypes
- Geometric alignment of user representations with the spectral space
- Computational feasibility analysis for large sparse graphs
- Temporal evaluation designed to prevent look-ahead leakage
- Explicit research questions, baselines, ablations, and diagnostic metrics

## Research questions

The proposal investigates whether explicit global graph structure can
improve exploratory recommendations compared with independently learned
item representations, and whether spectral representations can capture
long-range structure that local GNN neighborhoods miss.

## Reference

Yuan et al., **ContextGNN: Beyond Two-Tower Recommendation Systems**,
ICLR 2025.

[Read the full proposal](https://github.com/Aksinya-Bykova/Spectral-Discovery/blob/main/Yandex_Residency_Proposal%20(2).pdf)
