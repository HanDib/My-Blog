---
layout: page
title: Expeditions
---

{% for art in site.archives %}
<h2>{{ art.name }}: {{ art.country}} ({{ art.date_of_visit }})</h2>
<img src="{{ art. screenshot }}" alt="{{ art.name }}: {{ art.country}}">
{% for art in site.archives%}
<a href="{{ art.my_review_url }}">
<h2>{{ art.name }}: {{ art.country}} ({{ art.date_of_visit }})</h2>
<img src="{{ art.image }}" alt="{{ art.artist }}: {{ art.title}}">
</a>
{% endfor %}
{% endfor %}

