---
layout: page
title: 📅 Weekly Schedule
parent: 📜 Course Information
nav_order: 4
description: The weekly event schedule.
---

# Weekly Schedule

{% for schedule in site.schedules %}
{{ schedule }}
{% endfor %}
