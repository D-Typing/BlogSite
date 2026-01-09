---
layout: page
title: Home
---

# Cybersecurity Research & Write-ups

Focused on offensive security, malware analysis, and defensive techniques.

## Recent Write-ups

{% for writeup in site.writeups limit:5 %}

- [{{ writeup.title }}]({{ writeup.url }}) — {{ writeup.platform }}
  {% endfor %}

## Featured Projects

{% for project in site.projects limit:3 %}

- [{{ project.title }}]({{ project.url }})
  {% endfor %}
