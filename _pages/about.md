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
{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

<!-- New style rendering if publication categories are defined -->
{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h2>{{ category[1].title }}</h2><hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}
