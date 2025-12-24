---
layout: page
title: 📘 Exam 2 Lectures
description: Exam 2 Lectures
---

<div class="lecture-table-wrapper">
  <table>
    <thead>
      <tr>
        <th>#</th>
        <th>Date</th>
        <th>Module</th>
        <th>Lecture & Slides</th>
        <th>Activity & Key</th>
      </tr>
    </thead>
    <tbody>
      {% for l in site.data.exam2 %}
      <tr>
        <td>{{ l.number }}</td>
        <td>{{ l.date }}</td>
        <td> <a href="{{ site.baseurl }}/module/{{ l.number }}/"><strong>{{ l.lecture }}</strong></a></td>
        <td>
          Recording: <a href="{{ l.video }}">Blackboard</a><br>
          Slides: <a href="{{ l.slides_blank }}">Blank</a> / <a href="{{ l.slides_annotated }}">Annotated</a>
        </td>
        <td>
          Worksheet: <a href="{{ l.activity }}">{{ l.activity }}</a><br>
          Key: <a href="{{ l.activity_key }}">{{ l.activity }} Key</a>
        </td>
      </tr>
      {% endfor %}
    </tbody>
  </table>
</div>

<style>
table {
  table-layout: fixed;
  width: 100%;
  border-collapse: collapse;
}

table td, table th {
  padding: 4px 6px; 
  overflow: hidden; 
  text-overflow: ellipsis;
  white-space: nowrap; 
}

table td:first-child, table th:first-child { 
  width: 5%;
}

table td:nth-child(2), table th:nth-child(2) { 
  width: 12%;
}

table td:nth-child(3), table th:nth-child(3) {
  width: 25%;
}

table td:nth-child(4), table th:nth-child(4) { 
  width: 20%;
}

table td:nth-child(5), table th:nth-child(5) {
  width: 20%;
}

table th, table td {
  text-align: center;
}

table td:nth-child(4),
table td:nth-child(5) {
  text-align: left;
}
</style>