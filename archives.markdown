---
layout: page
title: Expeditions
---
{% for art in site.archives %}
<a href="{{art.url}}"> {{ art.name }}: {{ art.country}} ({{ art.date_of_visit }})</a>
<img src="{{ art. screenshot }}" alt= "{{ art.name }}: {{ art.country}}">
{% endfor %}

