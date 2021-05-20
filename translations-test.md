---
layout: default
title: Texts in Translation
permalink: /translationtest.html
---

### Texts in Translation

{% assign items_grouped = site.data.translations | group_by: 'century' | sort: 'title' %}
{% for group in items_grouped %}
<h3>{{group.name}} century</h3>
{% for item in group.items %}
<p><em>{{ item.title }}</em>{% if item.dates %} {{ item.dates }}{% endif %}. {{ item.info }}. Translation available at <a href="{{ item.url }}">{{ item.url }}</a></p>
{% endfor %}
{% endfor %}
