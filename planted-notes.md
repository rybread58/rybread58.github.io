---
layout: page
title: Planted Notes
permalink: /planted-notes/
---

{% for note in site.growing-notes %}
- [{{ note.title }}]({{ note.url }})
{% endfor %}
