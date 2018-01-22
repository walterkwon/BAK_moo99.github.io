---
layout: page
title: Archive
---

{% for post in site.posts %}{{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})  
{% endfor %}



<h1>Archive of posts with {{ page.type }} '{{ page.title }}'</h1>
<ul class="posts">
  {% for post in page.posts %}
    <li>
      <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
      <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
