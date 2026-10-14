---
layout: default
title: News
permalink: /news/
---

<ul class="news-list">
  {% for item in site.data.news %}
    <li>
      <time>{{ item.date | date: "%b %d, %Y" }}</time>
      <span>{{ item.text | markdownify | remove: '<p>' | remove: '</p>' }}</span>
    </li>
  {% endfor %}
</ul>
