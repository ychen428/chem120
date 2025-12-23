---
layout: page
title: 📘 Exam 1 Lectures
description: Listing of course modules and topics.
---
<div class="lecture-table-wrapper">
  <table>
    <thead>
      <tr>
        <th>#</th>
        <th>Date</th>
        <th>Lecture & Slides</th>
        <th>Activity & Key</th>
      </tr>
    </thead>
    <tbody>
      {% for l in site.data.exam1 %}
      <tr>
        <td>{{ l.number }}</td>
        <td>{{ l.date }}</td>
        <td>
          <a href="{{ site.baseurl }}/lectures/lecture{{ l.number }}/"><strong>{{ l.lecture }}</strong></a><br>
          Slides: <a href="{{ l.slides_blank }}">Blank</a> / <a href="{{ l.slides_annotated }}">Annotated</a>
        </td>
        <td>
          Worksheet: <a href="{{ l.activity_link }}">{{ l.activity }}</a> /
          Key: <a href="{{ l.key_link }}">{{ l.activity }} Key</a>
        </td>
      </tr>
      {% endfor %}
    </tbody>
  </table>
</div>


<style>
table {
  table-layout: fixed; /* forces widths */
  width: 100%;
  border-collapse: collapse; /* optional, tighter spacing */
}

table td, table th {
  padding: 4px 6px; /* reduce padding */
  overflow: hidden; /* truncate content if too long */
  text-overflow: ellipsis;
  white-space: nowrap; /* prevent wrapping */
}

table td:first-child, table th:first-child { /* # column */
  width: 5%;
}

table td:nth-child(2), table th:nth-child(2) { /* Date */
  width: 15%;
}

table td:nth-child(3), table th:nth-child(3) { /* Lecture */
  width: 38%;
}

table td:nth-child(4), table th:nth-child(4) { /* Activity */
  width: 45%;
}

table th:first-child, table td:first-child,
table th:nth-child(2), table td:nth-child(2) {
  text-align: center; /* center # and Date */
}

table th:nth-child(3), table td:nth-child(3),
table th:nth-child(4), table td:nth-child(4) {
  text-align: left;   /* left-align Lecture and Activity */
}

table th:nth-child(3), table th:nth-child(4) {
  text-align: center; /* Center Lecture and Activity headers */
}
</style>
