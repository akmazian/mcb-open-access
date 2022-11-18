---
permalink: "/courses/"
layout: page
title: Courses
nav_exclude: true
description: A directory containing all of the courses.
---

# Courses

{% assign courses = site.courses | reverse %}
{% for course in courses %}
{{ course }}
{{ note }}
{% endfor %}
