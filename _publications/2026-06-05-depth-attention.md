---
title: 'Depth-Attention: Cross-Layer Value Mixing for Language Models'
permalink: /publication/depth-attention/
date: '2026-06-05'
category: conferences
venue: EMNLP 2026
profile_order: 1
paperurl: https://arxiv.org/abs/2606.05014
codeurl: https://github.com/LUMIA-Group/Depth-Attention
authors: Boyi Zeng*, Yiqin Hao*, Zitong Wang, Shixiang Song, He Li, Feichen Song, Yifan Liu, Ziwei He, Xinbing Wang, Zhouhan Lin‡
excerpt: Enables content-based reuse of earlier-layer value representations inside attention. The current-layer query selects keys along depth and mixes their values before sequence attention, reusing standard Q/K/V and V-cache slots without extra parameters or persistent inference state.
result: On a 3B Qwen3-style model, lowers perplexity by 0.3 and improves average downstream accuracy by about 2 percentage points with negligible inference overhead.
collection: publications
profile_owner: true
---

## Method

Depth-Attention performs content-based selection along the depth dimension at the same token position. Before standard causal self-attention, the current-layer query attends to keys from earlier layers and mixes their values into the value state used by sequence attention. It reuses the standard attention projections and V-cache slots, without adding parameters or persistent inference state beyond the normal KV cache.

## Results

On a 3B Qwen3-style model, PPL decreases by 0.3 and average downstream accuracy improves by approximately 2 percentage points, with negligible inference overhead. The work also explores compatibility with mHC/iHC-style methods and has been cited in model releases by Nanbeige and Shanghai AI Laboratory.
