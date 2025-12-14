---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
---

{% assign projs = site.projects | sort: 'date' | reverse %}
{% for p in projs %}
### [{{ p.title }}]({{ p.url | relative_url }})
{{ p.one_liner }}

{% if p.links %}
**Links:** 
{% for l in p.links %}
[{{ l.label }}]({{ l.url }}){% unless forloop.last %} · {% endunless %}
{% endfor %}
{% endif %}

---
{% endfor %}
