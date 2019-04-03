---
title:  "Blogs"
layout: archive
permalink: /Blogs/
author_profile: true
comments: true
---

<h1>Latest Posts</h1>


<ul>
{% for post in site.posts %}
    {% if post.path contains 'blog' %}
    <li>
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt }}</p>
    </li>  
    {% endif %}
{% endfor %}
</ul>
