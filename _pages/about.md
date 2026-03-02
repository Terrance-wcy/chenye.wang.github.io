---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

👋 Hello, I am **Chenye Wang**.

I am a final-year master’s student at Beijing Normal University, advised by [Prof. Yongzhen Huang](https://scholar.google.com/citations?user=OH7-k7oAAAAJ&hl=en) and [Prof. Saihui Hou](https://scholar.google.com/citations?user=6gnHaLcAAAAJ&hl=en&oi=ao). I received my bachelor’s degree from Shandong University in June 2023. Recently, I’m interested in Vision-Language-Action Model.



<span class='anchor' id='research'></span>

# 🔬 Research Interests
- **Human-centered Computer Vision**: gait recognition and action recognition in unconstrained surveillance and UAV-view scenarios.
- **Multi-modal Representation Learning**: vision-language pre-training and cross-modal alignment (image–text), as well as multi-sensor retrieval(e.g., camera–LiDAR) for robust representation learning.
- **Label-efficient Learning**: semi-supervised, weakly-supervised and self-supervised learning for large-scale vision tasks.

<span class='anchor' id='news'></span>

# 🔥 News
- **[Feb. 2026]** 🎉 One paper accepted by CVPR 2026.
- **[Jan. 2026]** 🎉 One paper accepted by ICLR 2026.
- **[Nov. 2025]** 🎉 One paper accepted by IEEE TIFS.
- **[Jan. 2025]** 🎉 One paper accepted by AAAI 2025 and selected for oral presentation (Top 4.6%).
- **[Jul. 2024]** 🎉 One paper accepted by ACM MM 2024.
- **[2022–2023]** 🎉🎉 Multiple papers on hypergraph modeling and bioinformatics.

<span class='anchor' id='publications'></span>

# 📚 Publications
{% for link in site.data.publications.main %}
<div class='paper-box'>
  <div class='paper-box-text' markdown="1">
{% if link.conference_short %}<div class="badge">{{ link.conference_short }}</div>{% endif %}

**{{ link.title }}**

{{ link.authors }}

<em>{{ link.conference }}</em><br/>
<div class="pub-links">
{% if link.pdf %}<a href="{{ link.pdf }}">Paper</a>{% endif %}
{% if link.code %}<a href="{{ link.code }}">Code</a>{% endif %}
{% if link.bibtex %}<a href="{{ link.bibtex }}">BibTex</a>{% endif %}
</div>
{% if link.notes %} **{{ link.notes }}**{% endif %}
{% if link.others %} {{ link.others }}{% endif %}
  </div>
</div>
{% endfor %}

<span class='anchor' id='services'></span>

<span class='anchor' id='honors'></span>

# 🏅 Honors & Awards
- **Xiaomi Scholarship**, Dec 2025
- **Huawei Scholarship**, May 2025
- **Outstanding Graduate**, Shandong University, May 2023
- **1st Place**, The 4th International Competition on Human Identification at a Distance, Apr 2023


# 🤝 Services
#### Academic Services
- Reviewer for IEEE TIFS, PRCV, ICIG

#### University Service
- Excellent Teaching Assistant for Machine Learning (Beijing Normal University, 2024)
