---
layout: defaultmodern
title: Blog
---
 
<div class="card">
  <h2>Alle Beiträge</h2>
  <h5>Hier sehen Sie eine Übersicht über alle Blog-Beiträge auf meiner Website</h5>
</div>
{% for post in site.posts %}
<hr>
<div class="card">
  <h2>{{ post.title }}</h2>
  <h5>Erstellt am: <span>{{ post.date | date_to_string }}</span></h5>
  <div class="fakeimg" style="height:200px;">Image</div>          
  <p>Some text...  <a href="{{ post.url }}" title="{{ post.title }}">Lesen...</a></p>  
  </div>
{% endfor %}
