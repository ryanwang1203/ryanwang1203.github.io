---
layout: single
title: "Projects"
permalink: /projects/
author_profile: true
classes: wide
---

<div class="grid__wrapper">
{% assign projs = site.projects | sort: 'date' | reverse %}
{% for p in projs %}
  <div class="grid__item">
    <article class="archive__item" itemscope itemtype="https://schema.org/CreativeWork">
      <h2 class="archive__item-title no_toc" itemprop="headline" style="margin-top:0;">
        <a href="{{ p.url | relative_url }}">{{ p.title }}</a>
      </h2>

      {% assign blurb = p.one_liner | default: p.excerpt %}
      {% if blurb %}
      <p class="archive__item-excerpt" itemprop="description" style="margin-bottom:.6rem;">
        {{ blurb | strip_html }}
      </p>
      {% endif %}

      {% if p.links %}
      <p style="margin:0 0 .6rem 0;">
        {% for l in p.links %}
          <a class="btn btn--primary btn--small" href="{{ l.url }}" target="_blank" rel="noopener">
            {{ l.label }}
          </a>
        {% endfor %}
      </p>
      {% endif %}

      <p class="page__meta" style="margin:0;">
        <i class="far fa-calendar-alt" aria-hidden="true"></i>
        {{ p.date | date: "%b %Y" }}
      </p>
    </article>
  </div>
{% endfor %}
</div>
