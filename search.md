---
layout: page
title: Search
---


<script>
  (function() {
    var cx = '006842924949017232700:oenlz6r8hq8';
    var gcse = document.createElement('script');
    gcse.type = 'text/javascript';
    gcse.async = true;
    gcse.src = 'https://cse.google.com/cse.js?cx=' + cx;
    var s = document.getElementsByTagName('script')[0];
    s.parentNode.insertBefore(gcse, s);
  })();
</script>
<gcse:search></gcse:search>




  <div id="search-searchbar"></div>

  <div class="post-list" id="search-hits">
    {% for post in site.posts %}
      <div class="post-item">
        {% assign date_format = site.minima.date_format | default: "%b %-d, %Y" %}
        <span class="post-meta">{{ post.date | date: date_format }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h2>

        <div class="post-snippet">{{ post.excerpt }}</div>
      </div>
    {% endfor %}
  </div>

  {% include algolia.html %}
