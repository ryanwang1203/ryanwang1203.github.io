---
layout: single
title: "News"
permalink: /news/
author_profile: true
entries_layout: list
---

{% for post in site.posts %}
  {% include archive-single.html %}
{% endfor %}
