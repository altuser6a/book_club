---
layout: page
title: Posts
---

<ul>
  <li><a href="#Posts_by_Date"> by Date </a></li>
  <li><a href="#Posts_by_Tag"> by Tag</a></li>
</ul>

---

<div style="display: flex;">
<div style="flex: 50%;">

<h3 id="Posts_by_Date">Posts by Date</h3>
<ul>
  {% for post in site.posts %}
    <li>
      {{ post.date | date: "%b %m '%y" }} - <a href="{{ post.url }}">{{ post.title }}</a> 
    </li>
  {% endfor %}
</ul>

<h3 id="Posts_by_Tag">Posts by Tag</h3>
{% for tag in site.tags %}
  <h4>{{ tag[0] }}</h4>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

<!-- Splits the page into two columns, one for posts by date and posts by tag-->
<!--
<div style="display: flex;">
<div style="flex: 50%;">

<h3 id="Posts_by_Date">Posts by Date</h3>
<ul style="list-style: none; padding: 0; margin: 0;">
  {% for post in site.posts %}
    <li>
      {{ post.date | date: "%b %m '%y" }} - <a href="{{ post.url }}">{{ post.title }}</a> 
    </li>
  {% endfor %}
</ul>
</div>

<div>
  <h3 id="Posts_by_Tag">Posts by Tag</h3>
{% for tag in site.tags %}
  <h4>{{ tag[0] }}</h4>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
</div>
</div>
-->
