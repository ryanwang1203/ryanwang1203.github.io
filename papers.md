---
layout: single
title: "Papers"
permalink: /papers/
author_profile: true
---

{% assign pubs = site.publications | sort: 'date' | reverse %}
{% for p in pubs %}
### [{{ p.title }}]({{ p.url | relative_url }})
*{{ p.venue }}* — {{ p.date | date: "%b %Y" }}  
{{ p.citation }}

{% if p.links %}
**Links:** 
{% for l in p.links %}
[{{ l.label }}]({{ l.url }}){% unless forloop.last %} · {% endunless %}
{% endfor %}
{% endif %}

---
{% endfor %}
