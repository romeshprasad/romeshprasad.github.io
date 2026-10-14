---
layout: default
title: Publications
permalink: /publications/
---

{% if site.google_scholar != "" %}
<p class="muted">For a complete and up-to-date list, see <a href="{{ site.google_scholar }}">Google Scholar</a>.</p>
{% endif %}

{% assign by_year = site.data.publications | group_by: "year" | sort: "name" | reverse %}
{% for year in by_year %}
<section class="pub-year">
  <h2>{{ year.name }}</h2>
  <ol class="pub-list">
    {% for pub in year.items %}
    <li>
      <span class="pub-title">{{ pub.title }}</span>
      <span class="pub-authors">{{ pub.authors | markdownify | remove: '<p>' | remove: '</p>' }}</span>
      <span class="pub-venue"><em>{{ pub.venue }}</em>{% if pub.type %} <span class="tag">{{ pub.type }}</span>{% endif %}</span>
      <span class="pub-links">
        {% if pub.pdf and pub.pdf != "" %}<a href="{{ pub.pdf | relative_url }}">PDF</a>{% endif %}
        {% if pub.doi and pub.doi != "" %}<a href="https://doi.org/{{ pub.doi }}">DOI</a>{% endif %}
        {% if pub.code and pub.code != "" %}<a href="{{ pub.code }}">Code</a>{% endif %}
        {% if pub.data and pub.data != "" %}<a href="{{ pub.data }}">Data</a>{% endif %}
        {% if pub.slides and pub.slides != "" %}<a href="{{ pub.slides }}">Slides</a>{% endif %}
      </span>
    </li>
    {% endfor %}
  </ol>
</section>
{% endfor %}
