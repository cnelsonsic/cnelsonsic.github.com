---
layout: page
title: Blogs and Pages!
tagline: Because the internet needs more blog.
---
{% include JB/setup %}

Sometimes I write things:

<ul class="posts">
  {% for post in site.posts %}
    <li>
        <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
        &mdash;
        <em>&ldquo;{{ post.description }}&rdquo;</em>
        <sup>({{ post.date | date_to_string }})</sup>
    </li>
  {% endfor %}
</ul>
