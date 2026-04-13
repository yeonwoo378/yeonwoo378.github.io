---
permalink: /
title: "About Me."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a graduate student at KAIST, where I am fortunate to be advised by Professor [Seunghoon Hong](https://maga33.github.io/). My research interests lie in the advancement of Generative Models, with a specific focus on Flow Matching and Diffusion.

<div id="education"></div>

## Education
- **M.S. in Computer Science**, KAIST, South Korea, **2025–Present**
- **B.S. in Computer Science and Electronic Engineering (Double Major)**, KAIST, South Korea, **2021–2025**

<div id="publications"></div>

## Publications

{% include base_path %}

{% for post in site.publications reversed %}
{% include archive-single.html %}
{% endfor %}


{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

<div id="teaching"></div>

## Teaching

- **CS101** Introduction to Programming, Teaching Assistant, KAIST, 2022 Fall – 2024 Spring
- **CS371** Introduction to Deep Learning, Teaching Assistant, KAIST, 2025 Fall

<div id="academic-services"></div>

## Academic Services

- **Reviewer**: ICLR 2026, CVPR 2026
