---
layout: page
title: Works
permalink: /works/
category_name: works
---

{% assign tags = site.tags | sort %}
{% for tag in tags %}

<div style="display: inline-block;">
    <a href="/tag/{{ tag | first | slugify }}/">
            {{ tag[0] | replace:'-', ' ' | smartify }}
    </a> |
</div>

{% endfor %}

{% if page.category_name %}
  {% assign category_name = page.category_name %}
{% endif %}

<div class="container mx-auto">
  {% for post in site.categories[category_name] %}
    {% include post_block.html %}
  {% endfor %}
</div>
