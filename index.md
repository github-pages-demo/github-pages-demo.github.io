---
layout: default
title: GitHub Pages Demo
description: Demo site for GitHub Pages&#58; An Often Overlooked Platform presentation
---

This site is meant to accompany the GitHub Pages: An Often Overlooked Platform presentation.

## Blog Posts

{% for post in site.posts %}

### [{{ post.title }}]({{ post.url }})
{{ post.excerpt }}

{% endfor %}