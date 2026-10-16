---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

[Download my current CV (Chinese PDF)]({{ '/files/CV.pdf' | relative_url }})

## Education

**Shanghai Jiao Tong University (SJTU)** — Undergraduate<br>
September 2023 – Present · Shanghai, China

## Research Interests

Deep learning and large language model pretraining architectures, with a focus on looped Transformers, effective computational depth, latent reasoning, and adaptive computation.

## Experience

{% include profile-experience.html %}

## Papers

{% assign profile_pubs = site.publications | where: "profile_owner", true | sort: "profile_order" %}
{% for paper in profile_pubs %}
- **[{{ paper.title }}]({{ paper.url | relative_url }})** — {{ paper.venue }}.
{% endfor %}

## Languages

- English: CET-6, 646.
- French: DELF B2.

## Contact

[hyq718@sjtu.edu.cn](mailto:hyq718@sjtu.edu.cn) · [haoyiqin718@gmail.com](mailto:haoyiqin718@gmail.com)
