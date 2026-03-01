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

I am an M.E. student in Intelligence Science and Technology at Beijing Normal University, advised by Prof. Yongzhen Huang and Assoc. Prof. Saihui Hou. My research mainly focuses on gait recognition, biometrics, and human-centered computer vision.

<span class='anchor' id='education'></span>

# 🎓 Education
- **Beijing Normal University**, M.E. in Intelligence Science and Technology, Sept 2023 – Jun 2026  
  - GPA: 3.7/4.0  
  - Mentors: Prof. Yongzhen Huang, Assoc. Prof. Saihui Hou  
  - Coursework: Deep Learning, Machine Learning, Information Theory
- **Shandong University**, B.S. in Statistics, Sept 2019 – Jun 2023  
  - Selected for the Data Science and Artificial Intelligence Elite Program  
  - GPA: 89.52/100  
  - Coursework: Mathematical Analysis, Advanced Algebra, Probability Theory

<span class='anchor' id='research'></span>

# 🔬 Research Interests
- **Gait Recognition & Biometrics**
- **Computer Vision:** Human-centered vision, video understanding
- **Machine Learning:** Representation learning, semi-supervised learning
- **Generative Models & Diffusion Models**

<span class='anchor' id='news'></span>

# 🔥 News
- **[Feb. 2026]** 🎉 One paper accepted by CVPR 2026 (MMGait: Towards Multi-Modal Gait Recognition).
- **[Feb. 2026]** 🎉 One paper accepted by ICLR 2026 (GaitSnippet: Gait Recognition Beyond Unordered Sets and Ordered Sequences).
- **[Jan. 2025]** 🎉 One paper accepted by AAAI 2025 (RA-GAR: A Richly Annotated Benchmark for Gait Attribute Recognition, Oral).
- **[Oct. 2024]** 🎉 One paper accepted by ACM MM 2024 (AerialGait: Bridging Aerial and Ground Views for Gait Recognition).
- **[2022–2024]** 🎉 Multiple journal papers on hypergraph modeling and bioinformatics (BMC Bioinformatics, PLOS Computational Biology).

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
