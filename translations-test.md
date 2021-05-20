---
layout: default
title: Texts in Translation
permalink: /translationtest.html
---

### 3rd Century)

*De Singularitate Clericorum: A Third-century Treatise Against Spiritual Marriage* by an anonymous cleric; trans. Diane Shane Fruchtman. Published and hosted by EPISCOPUS, 15 Aug 2014. Download the PDF.

EPISCOPUS scholars are interested in the role of bishops & secular clergy in medieval society. Membership is currently *gratis* and includes updates on CFPs of interest to scholars doing research on medieval clergy, and an invitation to an annual business meeting at the International Congress on Medieval Studies in Kalamazoo, Michigan.

<a href="https://docs.google.com/forms/d/1azz1dyCwj6GlNZrg3zXIEzhUEV2KUf1FTYAQf-YGZXc/viewform">Click here</a> to join EPISCOPUS.

### Member Directory

{% assign items_grouped = site.data.translations | group_by: 'century' | sort: 'title' %}
{% for group in items_grouped %}
<h3>{{group.name}}</h3>
{% for item in site.data.items %}
<p><em>{{ item.title }}</em></p>{% if item.dates %} {{ item.dates }}{% endif %} {{ item.info }}. item available at <a href="{{ item.url }}">{{ item.url }}</a>
{% endfor %}
{% endfor %}
