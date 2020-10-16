---
layout: page
title: 🎤 Talks
permalink: /talks/
---

Giving a talk is a great responsability, why? The audience is giving you something they will never get back, their <b>time</b>. Here some of them:

<h4>Talks by date:</h4>

<ul>
  {% for post in site.categories.Talk %}
    
    <li><a href="{{ post.url }}">{{ post.title }} </a> <br> {{ post.tags | join: ", "}} |  {{ post.date | date: "%-d %b %Y" }}</li> <hr style="height:1pt; visibility:hidden;" />
    
  {% endfor %}
</ul>

---------------------------------------------------------------------------------

<h4>Talks by topic:</h4>

{% assign sorted_tags = site.tags | sort %}
{% for tag in sorted_tags %}
{% assign zz = tag[1] | where: "category", "Talk" | sort %}
{% if zz != empty %}
{% if tag.first[0] == null %}

<h5><span class="tag">{{ tag[0] }}</span></h5>
<ul>
  {% for p in zz %}
  <li><a href="{{ p.url }}">{{ p.title }}</a></li>

  {% endfor %}
 </ul>



 {% endif %}
 {% endif %}

 {% endfor %}