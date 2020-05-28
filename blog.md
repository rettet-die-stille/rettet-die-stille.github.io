---
layout: defaultmodern
title: Blog
---
 
<div class="card">
  <h1>Alle Beiträge</h1>
  <p>Hier sehen Sie eine Übersicht über alle Blog-Beiträge auf meiner Website</p>
</div>
{% for post in site.posts %}
<div class="card">
<hr>
<h1> 
 
   <a href="{{ post.url }}" title="{{ post.title }}"</a>
   
</h1>
<h5>Erstellt am: <span>{{ post.date | date_to_string }}</span></h5>
<p>{{post.shorttext}} &nbsp;<a href="{{ post.url }}" title="{{ post.title }}">Lesen...</a></p>  
</div>
{% endfor %}
