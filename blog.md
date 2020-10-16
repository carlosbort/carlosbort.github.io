---
layout: page
title: 📝 Blog
permalink: /blog/
---

Many times we do things. They happen, but they don't last. Writing is a way to give them constancy, spread the knowledge with others and learning for the future. Here are some things I have written:

<h4>Posts by date:</h4>

<ul>
  {% for post in site.categories.Post %}
    
    <li><a href="{{ post.url }}">{{ post.title }} </a> <br> {{ post.tags | join: ", "}} |  {{ post.date | date: "%-d %b %Y" }}</li> <hr style="height:1pt; visibility:hidden;" />
    
  {% endfor %}
</ul>

---------------------------------------------------------------------------------

<h4>Posts by topic:</h4>

{% assign sorted_tags = site.tags | sort %}
{% for tag in sorted_tags %}
{% assign zz = tag[1] | where: "category", "Post" | sort %}
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