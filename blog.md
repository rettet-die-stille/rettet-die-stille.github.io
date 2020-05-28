---
layout: defaultmodern
title: Blog
---
 
<div class="card">

## Alle Beiträge
  Hier sehen Sie eine Übersicht über alle Blog-Beiträge auf meiner Website.

</div>

{% for post in site.posts %}

<div class="card">
 
##{{ post.title }}
### Erstellt am: <span>{{ post.date | date_to_string }}</span>

   <div class="fakeimg" style="height:200px;">Image</div>          
   <p>Some text...  <a href="{{ post.url }}" title="{{ post.title }}">Lesen...</a></p>  
</div>

{% endfor %}
