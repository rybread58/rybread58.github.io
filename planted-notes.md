---
layout: page
title: Planted Notes
permalink: /planted-notes/
---

{% for note in site.planted-notes %}
- [{{ note.title }}]({{ note.url }})
{% endfor %}
