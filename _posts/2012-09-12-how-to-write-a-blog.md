---
layout: post
title: "Welcome to Jekyll!"
categories: classic hollywood
---

# Welcome

**Hello world**, this is my first Jekyll blog post.

I hope you like it!

... which is shown in the screenshot below:
![My helpful screenshot](/assets/screenshot.jpg)

... you can [get the PDF](/assets/mydoc.pdf) directly.

## Displaying an index of posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

## Tags

{% for tag in site.tags %}

  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

# Post excerpts

Excerpt with multiple paragraphs

Here's another paragraph in the excerpt.

<!--more-->

Out-of-excerpt

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
