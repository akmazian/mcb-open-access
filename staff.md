---
layout: page
title: The Team
description: A listing of all the team members working on the project.
---

# The Team

Staff information is stored in the `_staffers` directory and rendered according to the layout file, `_layouts/staffer.html`.

## Frontend

{% assign frontend = site.staffers | where: 'role', 'Frontend' %}
{% for member in frontend %}
{{ member }}
{% endfor %}

## Backend

{% assign backend = site.staffers | where: 'role', 'Backend' %}
{% for member in backend %}
{{ member }}
{% endfor %}

## Contributors

{% assign contributor = site.staffers | where: 'role', 'Contributor' %}
{% for member in contributor %}
{{ member }}
{% endfor %}






<!-- a sample if > for block

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}
## Teaching Assistants

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}

-->
