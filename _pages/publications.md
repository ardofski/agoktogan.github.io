---
layout: page
permalink: /publications/
title: publications
description: Papers and contest contributions, with links to public resources.
years: [2026, 2022, 2020]
nav: true
nav_order: 2
---

Read about [my contributions and research projects]({{ '/research/' | relative_url }}).

<div class="publications">
{% for y in page.years %}
  <h2 class="year">{{ y }}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>
