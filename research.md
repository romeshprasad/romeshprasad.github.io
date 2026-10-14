---
layout: default
title: Research
subtitle: "[One line summarizing the lab's research program.]"
permalink: /research/
---

{% for area in site.data.research %}
<section class="research-item">
  {% if area.image and area.image != "" %}
    <img src="{{ area.image | relative_url }}" alt="{{ area.title }}">
  {% endif %}
  <div>
    <h2>{{ area.title }}</h2>
    {{ area.description | markdownify }}
    {% if area.funding and area.funding != "" %}
      <p class="muted">Funding: {{ area.funding }}</p>
    {% endif %}
  </div>
</section>
{% endfor %}
