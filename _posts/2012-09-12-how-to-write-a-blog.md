---
layout: post
author: nhquydev
published: true
date: 2023-07-02 08:00:20 -0000
title: "Welcome to Jekyll!"
description: I created this beautiful looking Jekyll blog by forking a repository. You can also fork it to make it yours. Jekyll is a simple blog generator. The community is growing and the number of plugins is also growing. I have moved all my blogs to Jekyll!
categories: guidelines
tags: guidelines
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
