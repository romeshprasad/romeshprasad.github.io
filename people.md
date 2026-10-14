---
layout: default
title: People
permalink: /people/
---

{% assign groups = "pi:Principal Investigator|postdoc:Postdoctoral Researchers|phd:PhD Students|ms:MS Students|undergrad:Undergraduate Researchers" | split: "|" %}

{% for g in groups %}
  {% assign parts = g | split: ":" %}
  {% assign members = site.data.people | where: "group", parts[0] %}
  {% if members.size > 0 %}
  <section class="section">
    <h2>{{ parts[1] }}</h2>
    <div class="people-grid {% if parts[0] == 'pi' %}people-pi{% endif %}">
      {% for p in members %}
        <article class="person">
          <img src="{{ p.photo | relative_url }}" alt="Photo of {{ p.name }}">
          <div>
            <h3>{{ p.name }}</h3>
            <p class="muted">{{ p.role }}</p>
            {% if p.bio and p.bio != "" %}<p>{{ p.bio }}</p>{% endif %}
            <p class="person-links">
              {% if p.email and p.email != "" %}<a href="mailto:{{ p.email }}">Email</a>{% endif %}
              {% if p.website and p.website != "" %}<a href="{{ p.website }}">Website</a>{% endif %}
              {% if p.scholar and p.scholar != "" %}<a href="{{ p.scholar }}">Scholar</a>{% endif %}
            </p>
          </div>
        </article>
      {% endfor %}
    </div>
  </section>
  {% endif %}
{% endfor %}

{% assign alumni = site.data.people | where: "group", "alumni" %}
{% if alumni.size > 0 %}
<section class="section">
  <h2>Alumni</h2>
  <ul class="alumni-list">
    {% for p in alumni %}<li><strong>{{ p.name }}</strong> — {{ p.role }}</li>{% endfor %}
  </ul>
</section>
{% endif %}
