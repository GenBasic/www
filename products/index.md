---
layout: default
permalink: /products/
title: Products
description: >-
  The GenBasic catalogue — USB Wi-Fi and Bluetooth adapters and UL-listed
  power supplies for commercial and embedded deployment.
---

<section class="page-head">
  <p class="eyebrow">Catalogue</p>
  <h1>Products</h1>
  <p class="lede">
    Wireless adapters and power for single-board computers and embedded
    hosts. Each model number identifies one fixed specification.
  </p>
</section>

<section>
  <div class="grid three">
    {% assign products = site.pages | where: "type", "product" | sort: "order" %}
    {% for p in products %}
    <article class="card">
      <a class="card-link" href="{{ p.url | relative_url }}">
        <div class="shot">
          <img src="{{ p.image | relative_url }}" alt="{{ p.image_alt }}"
               width="{{ p.image_w }}" height="{{ p.image_h }}"
               loading="lazy" decoding="async">
        </div>
        <p class="pn">{{ p.model }}</p>
        <h2 class="card-title">{{ p.name }}</h2>
      </a>
      {% if p.highlights %}
      <ul class="highlights compact">
        {% for h in p.highlights %}<li>{{ h }}</li>{% endfor %}
      </ul>
      {% endif %}
      <p><a class="cta ghost small" href="{{ p.url | relative_url }}">Specifications</a></p>
    </article>
    {% endfor %}
  </div>
</section>
