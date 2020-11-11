---
layout: page
title: Artists
---
{% for artist in site.data.artists %}
<h2>{{ artist.ArtistID }}: {{ artist.EnglishName}} {{ artist.ChineseName }}</h2>
<p> {{artist.Nationality}}  {{artist.Gender}} {{artist.BirthYear}} {{artist.DeathYear}}</p>
{% for i in (1..3) %} 
<img src= "/media/china-artworks/{{ artist.EnglishName | replace: ' ' , '_' }}_/{{ artist.EnglishName | replace: ' ' , '_' }}_0{{ i }}.jpg">
  {{ i }}
{% endfor %}
{% endfor %}




