---
layout: page
title: Experience
permalink: /experience/
description: Industry, research, teaching, and professional service experience.
nav: true
nav_order: 4
display_categories: [work, research, teach, service]
---

{% if site.enable_work_categories and page.display_categories %}
  {% for category in page.display_categories %}
    <h2>{{ category | capitalize }}</h2>
    {% assign categorized_work = site.work | where: 'category', category %}
    {% assign sorted_work = categorized_work | sort: 'importance' %}
    {% for item in sorted_work %}
      {% include work.liquid item=item %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% assign sorted_work = site.work | sort: 'importance' %}
  {% for item in sorted_work %}
    {% include work.liquid item=item %}
  {% endfor %}
{% endif %}
