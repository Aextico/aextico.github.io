---
layout: home
title: "Blog"
---

{% for post in site.posts %}
<article style="margin-bottom: 2em;">
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <small>{{ post.date | date: "%d %B %Y" }}</small>
  <p>
    {{ post.excerpt | strip_html | truncate: 250 }}
    <a href="{{ post.url }}">Read more... →</a>
  </p>
</article>
{% endfor %}
