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

I am a final-year master’s student at Beijing Normal University, advised by [Prof. Yongzhen Huang](https://scholar.google.com/citations?user=OH7-k7oAAAAJ&hl=en) and [Prof. Saihui Hou](https://scholar.google.com/citations?user=6gnHaLcAAAAJ&hl=en&oi=ao). I received my bachelor’s degree from Shandong University in June 2023. My research mainly focuses on Human-centered Vision Task, Multi-modal Representation Learning and Label-efficient Learning.

<span class='anchor' id='research'></span>

# 🔬 Research Interests
- **Gait Recognition & Biometrics**
- **Computer Vision:** Human-centered vision, video understanding
- **Machine Learning:** Representation learning, semi-supervised learning
- **Generative Models & Diffusion Models**

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
  <div class='paper-box-image'>
    <div>
      {% if link.conference_short %}
      <div class="badge">{{ link.conference_short }}</div>
      {% endif %}
      {% if link.image %}
      <img src='{{ link.image }}' alt='{{ link.title }}' width="100%">
      {% endif %}
    </div>
  </div>

  <div class='paper-box-text' markdown="1">
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

# 🤝 Services
#### Academic Services
- Reviewer for IEEE TIFS, PRCV, ICIG

#### University Service
- Excellent Teaching Assistant for Machine Learning (Beijing Normal University, 2024)
