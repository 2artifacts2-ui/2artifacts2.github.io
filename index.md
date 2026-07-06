---
layout: default
title: My News Portal
---

# Latest News

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p>{{ post.date | date: "%B %d, %Y" }}</p>
    <div class="entry">
      {{ post.excerpt }}
    </div>
  </article>
{% endfor %}
