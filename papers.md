---
layout: single
title: "Papers"
permalink: /papers/
author_profile: true
---

{% assign pubs = site.publications | sort: 'date' | reverse %}
{% for p in pubs %}

{% assign out = nil %}
{% if p.links %}
  {% for l in p.links %}
    {% assign lab = l.label | downcase %}
    {% if lab == "paper" or lab == "doi" or lab == "pdf" %}
      {% assign out = l.url %}
    {% endif %}
  {% endfor %}
  {% if out == nil %}
    {% assign out = p.links[0].url %}
  {% endif %}
{% endif %}

### {% if out %}<a href="{{ out }}" target="_blank" rel="noopener">{{ p.title }}</a>{% else %}<a href="{{ p.url | relative_url }}">{{ p.title }}</a>{% endif %}

*{{ p.venue }}* — {{ p.date | date: "%b %Y" }}  
{{ p.citation }}

---

{% endfor %}
