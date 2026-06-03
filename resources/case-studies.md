---
layout: page
title: "AI & Data Case Studies | Apex Data Cloud"
description: "Case studies showing how Apex Data Cloud helps companies turn AI, machine learning, and data into measurable business results."
eyebrow: "Case Studies"
breadcrumb_name: "Case Studies"
permalink: /resources/case-studies/
keywords: "AI case studies, machine learning case studies, data analytics case studies, RAG case study, marketing analytics results"
sidebar: false
tldr: "Real-world examples of how Apex Data Cloud turns AI and data into measurable outcomes — churn reduction, RAG assistants, cloud savings, and attribution clarity."
cta_title: "Want results like these?"
---

{% if site.case_studies.size > 0 %}
<div class="post-list">
  {% for cs in site.case_studies %}
  <a class="post-card" href="{{ cs.url }}">
    <div class="post-meta">{{ cs.industry | default: "Case Study" }}</div>
    <h3>{{ cs.title | split: "|" | first | strip }}</h3>
    <p>{{ cs.description | truncate: 150 }}</p>
  </a>
  {% endfor %}
</div>
{% else %}
<p>Case studies are publishing soon. To discuss results we've delivered for companies like yours, <a href="/contact/">book a consultation</a>.</p>
{% endif %}
