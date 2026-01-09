---
layout: page
title: Projects
permalink: /projects/
---

A selection of technical projects related to cybersecurity, tooling, and research.

---

{% for project in site.projects %}

## [{{ project.title }}]({{ project.url }})

{{ project.description }}

{% if project.technologies %}
**Technologies:** {{ project.technologies | join: ", " }}
{% endif %}

---

{% endfor %}
