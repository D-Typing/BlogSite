---
layout: page
title: Write-ups
permalink: /writeups/
---

Technical write-ups covering labs, vulnerabilities, and security research.

---

{% for writeup in site.writeups %}

## [{{ writeup.title }}]({{ writeup.url }})

- **Platform:** {{ writeup.platform }}
- **Difficulty:** {{ writeup.difficulty }}
- **Date:** {{ writeup.date | date: "%Y-%m-%d" }}

{% if writeup.tags %}
**Tags:** {{ writeup.tags | join: ", " }}
{% endif %}

---

{% endfor %}
