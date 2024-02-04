---
layout: work
title: "human rights"
tag: human-rights
---

{% for tag in site.tags %}
  <a href="/work/{{ tag[0] }}/">{{ tag[0] }}</a>
{% endfor %}
