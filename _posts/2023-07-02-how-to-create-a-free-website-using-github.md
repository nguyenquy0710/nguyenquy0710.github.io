---
layout: post
author: nhquydev
published: true
date: 2023-07-02 08:00:20 -0000
title: "How to create a free website using github"
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
{{ myimage.path }}
{% endfor %}
