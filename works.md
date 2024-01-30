---
layout: category_index
title: Works
permalink: /works/
category_name: works
---

 {% for tag in site.categories %}
    <a href="#{{ tag[0] | slugify }}" class="post-tag">{{ tag[0] }}</a>
    {% endfor %}
