---
layout: category_index
title: Works
permalink: /works/
category_name: works
---

<ul class="mt-1 mt-lg-2 mr-2 mr-lg-3">
      {% for posts in site.tags.journalism %}
        {% if post.tags.journalism %}
        <li class="inline-block block-lg text-right ml-1 ml-lg-0">
          <a class="italic no-underline h4" href="{{ my_page.url | prepend: site.baseurl }}">
            {{ post.title }}
          </a>
        </li>
        {% endif %}
      {% endfor %}
    </ul>
