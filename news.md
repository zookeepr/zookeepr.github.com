---
layout: default
title: 'Zookeepr: News'
---

# News

{% assign firstpost = site.posts.first %}

## [{{ firstpost.title }}]( {{firstpost.url }})

{{ firstpost.content }}


{% for post in site.posts limit: 3 offset: 1%} 
## [{{ post.title }}]({{ post.url }})

  {{ post.content | truncate: 450 }}

  <a id="more" href="{{ post.url }}">Read More &raquo;</a>

{% endfor %}

<ul>
  {% for post in site.posts offset: 3 %}
    <li>
      <span>{{ post.date | date_to_string }}</span>
      &raquo;
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>



