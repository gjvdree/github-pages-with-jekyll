---
title: "Welcome to my nerdy blog"
---

I'm glad you are here. I plan to talk about ...


<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
