---
layout: category_index
title: Works
permalink: /works/
category_name: works
---

{% for post in site.tags.literature %}
<h2>{{ post.title }}</h2>
{% endfor %}
