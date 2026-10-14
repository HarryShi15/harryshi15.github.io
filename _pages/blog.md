---
layout: page
title: blog
permalink: /blog/
nav: true
nav_order: 2
---

{% if site.posts.size > 0 %}
{% for post in site.posts %}
## [{{ post.title }}]({{ post.url | relative_url }})

{{ post.date | date: "%B %d, %Y" }} · {{ post.description }}

{% endfor %}
{% else %}
Posts will appear here as they become available.
{% endif %}
