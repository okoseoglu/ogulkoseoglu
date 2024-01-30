---
layout: category_index
title: Works
permalink: /works/
category_name: works
---

{% raw %} {% for tag in site.tags %} {% assign tagName = tag | first | downcase %} {% assign postsCount = tag | last | size %} <li><a href='/tags?tagName={{ tagName }}'><i class='glyphicon glyphicon-tag'></i>{{ tagName }}</a>({{ postsCount }})</li> {% endfor %} {% endraw %}

