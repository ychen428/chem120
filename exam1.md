---
layout: page
title: Exam 1 Lectures
description: Listing of course modules and topics.
---

{% assign exam1_module = site.modules | where: "slug", "exam1" | first %}
{{ exam1_module }}