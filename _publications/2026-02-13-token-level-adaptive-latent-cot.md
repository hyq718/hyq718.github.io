---
title: Pretraining with Token-Level Adaptive Latent Chain-of-Thought
permalink: /publication/token-level-adaptive-latent-cot/
date: '2026-02-13'
category: preprints
venue: Under Review
profile_order: 3
paperurl: https://arxiv.org/abs/2602.08220
authors: Boyi Zeng*, Yiqin Hao*, He Li, Shixiang Song, Feichen Song, Zitong Wang, Siyuan Huang, Yi Xu, ZiWei He, Xinbing Wang, Zhouhan Lin‡
excerpt: 'Learns variable-length latent reasoning before each token during single-stage pretraining: harder tokens receive more computation and easier ones halt earlier. Parallel masking and a correctness-aware adaptive loss make token-level compute allocation trainable on general text.'
result: Achieves lower perplexity with fewer FLOPs across model scales and improves downstream performance under comparable compute budgets.
collection: publications
profile_owner: true
citation: Zeng, Boyi*, Hao, Yiqin*, et al. (2026). &quot;Pretraining with Token-Level Adaptive Latent Chain-of-Thought.&quot; arXiv preprint.
---

## Method

The model learns a variable-length latent chain of thought before emitting each token, spending longer on difficult positions and halting early on easier ones. Parallel attention masking organizes the dependencies over token positions and latent steps, while a correctness-aware adaptive loss trains the halting behavior during single-stage pretraining on general text.

## Results

Across model scales, adaptive latent computation attains lower perplexity with fewer FLOPs and improves downstream performance under comparable compute budgets.
