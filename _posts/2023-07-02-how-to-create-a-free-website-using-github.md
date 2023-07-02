---
layout: post
title: "How to create a free website using github"
date: 2023-07-02 08:00:20 -0000
categories: CATEGORY-1 CATEGORY-2
author: nhquydev
---

{% assign author = site.data.people[page.author] %}
<a rel="author"
  href="https://twitter.com/{{ author.twitter }}"
  title="{{ author.name }}">
{{ author.name }}
</a>

{% assign image_files = site.static_files | where: "image", true %}
{% for myimage in image_files %}
{{ myimage.path }}
{% endfor %}
