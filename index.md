---
layout: page
title: wildermuthn
tagline: Adventures in Lisp
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
   {% unless post.draft %}
    <li><span>{{ post.date | date_to_string }}</span> <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
   {% endunless %}
  {% endfor %}
</ul>
