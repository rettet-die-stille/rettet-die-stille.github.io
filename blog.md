---
layout: defaultmodern
title: Blog
---
 
 <div class="card">
  <h2>Alle Beiträge</h2>
  Hier sehen Sie eine Übersicht über alle Blog-Beiträge auf meiner Website.
</div>

{% for post in site.posts %}

<div class="card">
  <h2>{{ post.title }}</h2>
  <h5><span>{{ post.date | date_to_string }}</span> » <a href="{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a></h5>
  <div class="fakeimg" style="height:200px;">Image</div>          
  <p>Some text..</p>
</div>

{% endfor %}
