---
layout: default
permalink: /products/
title: Products
description: >-
  The GenBasic catalogue — RF wireless adapters and power supplies for
  commercial and embedded deployment.
---

<section class="page-head">
  <p class="eyebrow">Catalogue</p>
  <h1>Products</h1>
  <p class="lede">
    Wireless adapters and power for single-board computers and embedded
    hosts. Each model number identifies one fixed specification.
  </p>
</section>

{% assign families = site.pages | where: "layout", "family" | sort: "family" %}
{% for f in families %}
<section class="family-block">
  <div class="family-head">
    <div>
      <h2>{{ f.heading }} <span class="family-sub">{{ f.eyebrow }}</span></h2>
      <p>{{ f.intro }}</p>
    </div>
    <a class="cta ghost small" href="{{ f.url | relative_url }}">All {{ f.family_label }} &rarr;</a>
  </div>

  <div class="grid three">
    {% assign items = site.pages | where: "type", "product" | where: "family", f.family | sort: "order" %}
    {% for p in items %}
    <article class="card">
      <a class="card-link" href="{{ p.url | relative_url }}">
        <div class="shot">
          <img src="{{ p.image | relative_url }}" alt="{{ p.image_alt }}"
               width="{{ p.image_w }}" height="{{ p.image_h }}"
               loading="lazy" decoding="async">
        </div>
        <p class="pn">{{ p.model }}</p>
        <h3 class="card-title">{{ p.name }}</h3>
      </a>
      {% if p.highlights %}
      <ul class="highlights compact">
        {% for h in p.highlights %}<li>{{ h }}</li>{% endfor %}
      </ul>
      {% endif %}
      <p class="card-actions">
        <a class="cta buy" href="{{ p.buy }}">Buy on Amazon</a>
        <a class="spec-link" href="{{ p.url | relative_url }}">Full specifications &rarr;</a>
      </p>
    </article>
    {% endfor %}
  </div>
</section>
{% endfor %}
