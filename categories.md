---
layout: page
title: Categories
permalink: /categories/
---

<ul>
  {% for category in site.categories %}
    <li>
      <a href="/categories/{{ category[0] | uri_escape }}/">
        {{ category[0] }} ({{ category[1].size }})
      </a>
    </li>
  {% endfor %}
</ul>
