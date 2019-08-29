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

## Contact Me

<form action="https://formspree.io/cole.mike@gmail.com" method="POST">
    <div>
        <label for="name">Name: </label>
        <input type="text" id="name" name="name" />
    </div>
    <div>
        <label for="email">Email: </label>
        <input type="text" id="email" name="email" />
    </div>
    <div>
        <label for="comments">Comments: </label>
        <textarea id="comments" name="comments"></textarea>
    </div>
    <div><input type="submit" value="Send" /></div>
</form>