---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

I am interested in the interaction of multiple learning pathways, both from an algorithmic perspective, as well as uncovering the multi-regional circuits that underlie learning. I study the neural dynamics that emerge over learning to support new task-relevant computations, with a focus on how feedback - sensory and internal feedback loops - can flexibly modulate effective cortical dynamics, and how these input-driven dynamics are learnt via multiple forms of errors. 

Across projects, I integrate data-driven and/or normative modeling of behavioral strategies to analyze neural data in light of the actual computations at play and to better understand variability across individuals.

I am also motivated by a dynamical systems perspective that understanding neural computation requires not only identifying neural representations, but also uncovering the rules that govern how those representations evolve over time.

## Projects

{% include base_path %}
{% assign research_projects = site.portfolio | sort: "order" %}
<div class="grid__wrapper">
{% for post in research_projects %}
    {% include archive-single.html type="grid" %}
{% endfor %}
</div>
<div class="cf"></div>
