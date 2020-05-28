---
layout: defaultmodern
title: Blog
---
 
<div class="card">
  <h2>Alle Beiträge</h2>
  <p>Hier sehen Sie eine Übersicht über alle Blog-Beiträge auf meiner Website</p>
</div>

{% for post in site.posts %}

<div class="card">
 
  <h2>{{ post.title }}</h2>
  <p>Erstellt am: <span>{{ post.date | date_to_string }}</span></p>
  <div class="fakeimg" style="height:200px;">Image</div>          
  <p>Some text...  <a href="{{ post.url }}" title="{{ post.title }}">Lesen...</a></p>  
  </div>

{% endfor %}
