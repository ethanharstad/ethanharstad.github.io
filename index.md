---
layout: page
title: Ravings of a Mad Engineer
tagline: High altitude ballooning, robotics, UAS, communications
---
[GitHub](https://github.com/ethanharstad) - 
[@nv1k](https://twitter.com/NV1K) - 
[Google+](https://plus.google.com/113570820998505644644/posts)

## Recent Posts

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
