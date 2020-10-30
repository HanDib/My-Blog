---
layout: page
title: Artists
---

{% for artist in site.data.artists %}
<h2>{{ artist.ArtistID }}: {{ artist.EnglishName}} {{ artist.ChineseName }}</h2>
<p> {{artist.Nationality}}  {{artist.Gender}} {{artist.BirthYear}} {{artist.DeathYear}}</p>
<img src= "\media\china-artworks\{{ artist.EnglishName | replace: ' ' , '_' }}_{{ artist.ChineseName }}\{{ artist.EnglishName | replace: ' ' , '_' }}.jpg">
{% for i in (01..03) %} 
\media\china-artworks\{{ artist.EnglishName | replace: ' ' , '_' }}_{{ artist.ChineseName }}\{{ artist.EnglishName | replace: ' ' , '_' }}_0{{ i }}.jpg
  {{ i }}
{% endfor %}
{% endfor %}





