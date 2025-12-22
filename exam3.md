---
layout: page
title: Exam 3 Lectures
description: Listing of course modules and topics.
---

{% assign exam1_module = site.modules | where: "slug", "exam3" | first %}
{{ exam1_module }}