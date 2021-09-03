---
layout: default
permalink: /member-directory/
title: "EPISCOPUS: Membershiup"
---

EPISCOPUS scholars are interested in the role of bishops & secular clergy in medieval society. Membership is currently *gratis* and includes updates on CFPs of interest to scholars doing research on medieval clergy, and an invitation to an annual business meeting at the International Congress on Medieval Studies in Kalamazoo, Michigan.

<a href="https://docs.google.com/forms/d/1azz1dyCwj6GlNZrg3zXIEzhUEV2KUf1FTYAQf-YGZXc/viewform">Click here</a> to join EPISCOPUS.

### Member Directory

<ul>
{% assign memberlist = site.data.members | sort: 'last' %}
{% for member in memberlist %}
<li>{% if member.url %}<a href="{{ member.url }}">{% endif %}{{ member.first }} {{ member.last }}{% if member.url %}</a>{% endif %}{% if member.affiliation %}, {{ member.affiliation }}{% endif %}{% if member.country %} ({{ member.country }}){% endif %}{% if member.email %}, {{ member.email }}{% endif %}</li>
{% endfor %}
</ul>