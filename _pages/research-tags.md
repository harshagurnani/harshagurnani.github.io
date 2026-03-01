---
layout: archive
title: "Research by Tag"
permalink: /research-tags/
author_profile: true
---

{% include base_path %}
{% include group-by-array collection=site.portfolio field="tags" %}

{% for tag in group_names %}
  {% assign projects = group_items[forloop.index0] %}
  <h2 id="{{ tag | slugify }}" class="archive__subtitle">{{ tag }}</h2>
  <div class="grid__wrapper">
  {% for post in projects %}
    {% include archive-single.html type="grid" %}
  {% endfor %}
  </div>
{% endfor %}
