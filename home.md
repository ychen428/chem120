---
layout: page
title: 🏠 Home
permalink: /
nav_order: 1
---
# Chem 120 Fall 2025

**Instructors:** Yuting Chen **Lecture:** MWF 11–12pm, SCCT G027

## 📣 Latest Announcements

{% assign anns = site.announcements | sort: "date" | reverse | slice: 0,3 %}

{% for a in anns %}
**{{ a.title }}**  
<span class="text-small">{{ a.date | date: "%b %d" }}</span>  
{{ a.content }}
{% endfor %}


## Quick Links

[Blackboard](https://blackboard.hamilton.edu){: .btn .btn-outline }
[Gradescope](https://www.gradescope.com){: .btn .btn-outline }