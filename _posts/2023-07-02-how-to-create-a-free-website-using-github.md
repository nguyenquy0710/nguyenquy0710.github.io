---
layout: post
author: nhquydev
published: true
date: 2023-07-02 08:00:20 -0000
title: "How to create a free website using github"
description: I created this beautiful looking Jekyll blog by forking a repository. You can also fork it to make it yours. Jekyll is a simple blog generator. The community is growing and the number of plugins is also growing. I have moved all my blogs to Jekyll!
# permalink: /year/month/day/title.html
categories: guidelines github
tags: github
---

{% assign author = site.data.people[page.author] %}
<a rel="author"
  href="https://twitter.com/{{ author.twitter }}"
  title="{{ author.name }}">
{{ author.name }}
</a>

{% assign image_files = site.static_files %}
{% for myimage in image_files %}
{{ myimage.path | absolute_url }}
{% endfor %}
