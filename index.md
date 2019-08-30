---
layout: default
title: GitHub Pages Demo
description: Demo site for GitHub Pages&#58; An Often Overlooked Platform presentation
---

This site is meant to accompany the GitHub Pages: An Often Overlooked Platform presentation.

## Blog Posts
[Feed](/blog-feed.json)

{% for post in site.posts %}

### [{{ post.title }}]({{ post.url }})
{{ post.excerpt }}

{% endfor %}

## Blog Authors

{% for author in site.authors %}

### {{ author.name }}
![profile pic]({{ author.pic }})

From {{ author.location }}

{% endfor %}

## Favorite Movie Characters
{% for character in site.data.characters %}

- {{ character.character }} ({{ character.actor }}) in {{ character.movie }}

{% endfor %}

## Favorite Books
{% for book in site.data.books %}

- {{ book.title }} by {{ book.author }} ({{ book.published }})

{% endfor %}

## Contact Me

{% include contact.html %}