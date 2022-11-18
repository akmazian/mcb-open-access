---
permalink: "/available_classes/"
layout: page
title: Available Classes
has_children: true
description: List of All Available Classes
---

# Available Classes

{% assign courses = site.courses %}
{% for course in courses %}
{{ course }}
{{ course.note }}
{% endfor %}