---
layout: home
title: Welcome to My Jekyll Site
---

# Welcome to My Jekyll Site

This is the homepage of my Jekyll site. You can customize this page by editing the `index.md` file in your repository.

## Latest Blog Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}
