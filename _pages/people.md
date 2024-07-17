---
layout: archive
title: "People"
permalink: /people/
author_profile: false
redirect_from:
  - /resume
---

{% include base_path %}

{% assign sortedpeople = site.people | sort: 'order' %}

{% for post in sortedpeople %}
    {% include archive-single-people.html %}
  {% endfor %}

## PhD Student:

{% assign PhDpeople = site.people | where: "position", "PhD Student" %}

{% for post in PhDpeople %}
    {% include archive-single-people.html %}
  {% endfor %}



