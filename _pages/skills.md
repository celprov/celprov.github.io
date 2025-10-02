---
layout: page
title: "Skills"
description: "Overview of my technical skills and their application across projects."
nav: true
nav_order: 4
display_categories: ["work"]
horizontal: false
---

{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized skills -->
  {% for category in page.display_categories %}
  {% assign categorized_skills = site.skills | where: "category", category %}
  {% assign sorted_skills = categorized_skills | sort: "slug" %}
  <!-- Generate cards for each skill -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for skill in sorted_skills %}
      {% include skills_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for skill in sorted_skills %}
      {% include skills.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display skills without categories -->

{% assign sorted_skills = site.skills | sort: "slug" %}

  <!-- Generate cards for each skill -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for skill in sorted_skills %}
      {% include skills_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for skill in sorted_skills %}
      {% include skills.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
