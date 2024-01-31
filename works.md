---
layout: page
title: Works
permalink: /works/
category_name: works
---

{% assign tags = site.tags | sort %}
{% for tag in tags %}
 <p class="site-tag">
    <a href="/tag/{{ tag | first | slugify }}/"
        style="font-size: {{ tag | last | size  |  times: 4 | plus: 80  }}%">
            {{ tag[0] | replace:'-', ' ' }}
    </a>
</p>
{% endfor %}

{% if page.category_name %}
  {% assign category_name = page.category_name %}
{% endif %}

<div class="container mx-auto">
  {% for post in site.categories[category_name] %}
    {% include post_block.html %}
  {% endfor %}
</div>
