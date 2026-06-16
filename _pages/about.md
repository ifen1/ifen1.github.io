---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Ph.D. student in Computer Science and Engineering at the **Hong Kong University of Science and Technology (HKUST)**, advised by Prof. Shuai Wang. I completed a combined B.Eng.–M.Eng. program at the **China University of Petroleum (East China)** under Prof. Honglong Chen, and was previously a Research Assistant at the **College of William & Mary** with Prof. Huajie Shao (2023–2024), where my work on energy-based backdoor defense was published at ICML 2024.

My research centers on **AI security** — spanning LLM & agent security, backdoor attacks and defenses, embodied AI security, and trustworthy machine learning.

**Research interests:** AI Security · LLM & Agent Security · Embodied AI Security · Trustworthy Machine Learning

Publications
======
{% for post in site.publications reversed %}
<p style="margin-bottom:0.9em;">
{% if post.paperurl %}<a href="{{ post.paperurl }}"><b>{{ post.title }}</b></a>{% else %}<b>{{ post.title }}</b>{% endif %}<br>
<span style="font-size:0.92em;">{{ post.authors }}. <i>{{ post.venue }}</i>, {{ post.date | date: "%Y" }}.{% if post.tag and post.tag != "" %} <span style="color:#2a7ae2;font-weight:600;">{{ post.tag }}</span>{% endif %}</span>
</p>
{% endfor %}

Education
======
* **Ph.D. in Computer Science and Engineering**, HKUST, 2025 – Present
  * Advisor: Prof. Shuai Wang

Honors & Awards
======
* **National Scholarship** (Top 1%, ×3), Ministry of Education — 2021–2024
* **Outstanding Undergraduate Thesis** — 2025
* **Best Paper Award**, ICTC — 2024
* **First Prize**, Chinese Mathematics Competitions (CMC) — 2020

Academic Service
======
* **Journal Reviewer:** IEEE TIFS, IEEE TDSC, IEEE TNNLS, Pattern Recognition, ESWA, EAAI
* **Conference Reviewer:** NeurIPS, ACM MM
* **Sub-reviewer:** ACM CCS, USENIX Security, FSE
