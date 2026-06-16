---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Ph.D. student in Computer Science and Engineering at the **Hong Kong University of Science and Technology (HKUST)**, advised by [Prof. Shuai Wang](https://home.cse.ust.hk/~shuaiw/). I completed a combined B.Eng.–M.Eng. program at the China University of Petroleum (East China) under Prof. Honglong Chen, and was previously a Research Assistant at the College of William & Mary with Prof. Huajie Shao (2023–2024).

My research centers on **AI security** — spanning LLM & agent security, embodied AI security, and trustworthy machine learning.

Publications
======
{% assign pre = site.publications | where: "group", "preprint" | sort: "date" | reverse %}
{% for post in pre %}
<p style="margin-bottom:0.9em;">
{% if post.paperurl %}<a href="{{ post.paperurl }}"><b>{{ post.title }}</b></a>{% else %}<b>{{ post.title }}</b>{% endif %}<br>
<span style="font-size:0.92em;">{{ post.authors }}. <i>{{ post.venue }}</i>, {{ post.date | date: "%Y" }}.{% if post.tag and post.tag != "" %} <span style="background:#14507a;color:#fff;font-weight:700;font-size:0.78em;letter-spacing:0.4px;padding:2px 7px;border-radius:4px;vertical-align:middle;">{{ post.tag }}</span>{% endif %}</span>
</p>
{% endfor %}

{% assign mains = site.publications | where: "group", "main" | sort: "date" | reverse %}
{% for post in mains %}
<p style="margin-bottom:0.9em;">
{% if post.paperurl %}<a href="{{ post.paperurl }}"><b>{{ post.title }}</b></a>{% else %}<b>{{ post.title }}</b>{% endif %}<br>
<span style="font-size:0.92em;">{{ post.authors }}. <i>{{ post.venue }}</i>, {{ post.date | date: "%Y" }}.{% if post.tag and post.tag != "" %} <span style="background:#14507a;color:#fff;font-weight:700;font-size:0.78em;letter-spacing:0.4px;padding:2px 7px;border-radius:4px;vertical-align:middle;">{{ post.tag }}</span>{% endif %}</span>
</p>
{% endfor %}

{% assign corr = site.publications | where: "group", "corresponding" | sort: "date" | reverse %}
{% for post in corr %}
<p style="margin-bottom:0.9em;">
{% if post.paperurl %}<a href="{{ post.paperurl }}"><b>{{ post.title }}</b></a>{% else %}<b>{{ post.title }}</b>{% endif %}<br>
<span style="font-size:0.92em;">{% if post.authors and post.authors != "" %}{{ post.authors }}. {% endif %}<i>{{ post.venue }}</i>, {{ post.date | date: "%Y" }}. <b>corresponding author</b>{% if post.tag and post.tag != "" %} <span style="background:#14507a;color:#fff;font-weight:700;font-size:0.78em;letter-spacing:0.4px;padding:2px 7px;border-radius:4px;vertical-align:middle;">{{ post.tag }}</span>{% endif %}</span>
</p>
{% endfor %}

{% assign awd = site.publications | where: "group", "award" | sort: "date" | reverse %}
{% for post in awd %}
<p style="margin-bottom:0.9em;">
{% if post.paperurl %}<a href="{{ post.paperurl }}"><b>{{ post.title }}</b></a>{% else %}<b>{{ post.title }}</b>{% endif %}<br>
<span style="font-size:0.92em;">{{ post.authors }}. <i>{{ post.venue }}</i>, {{ post.date | date: "%Y" }}. <span style="background:#b04a1f;color:#fff;font-weight:700;font-size:0.78em;letter-spacing:0.4px;padding:2px 7px;border-radius:4px;vertical-align:middle;">Best Paper Award</span></span>
</p>
{% endfor %}

Honors & Awards
======
* **National Scholarship** (Top 1%, ×3), Ministry of Education — 2020, 2021 & 2024
* **Outstanding Undergraduate Thesis** — 2025
* **Best Paper Award**, ICTC — 2024
* **First Prize**, Chinese Mathematics Competitions (CMC) — 2020

Academic Service
======
* **Journal Reviewer:** IEEE TIFS, IEEE TDSC, IEEE TNNLS, Pattern Recognition, ESWA, EAAI
* **Conference Reviewer:** NeurIPS, ACM MM
* **Sub-reviewer:** ACM CCS, USENIX Security, FSE
