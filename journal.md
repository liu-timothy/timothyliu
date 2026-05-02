---
layout: default
title: Journal
permalink: /journal/
---

# My Journal

{% for post in site.posts %}
## [{{ post.title }}]({{ post.url }})
*{{ post.date | date: "%B %d, %Y" }}*

{{ post.excerpt }}
[Read more →]({{ post.url }})

---
{% endfor %}

{% if site.posts.size == 0 %}
*No journal entries yet. Check back soon for my first post!*
{% endif %}
