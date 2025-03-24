---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
{% raw %}{% assign educations = site.data.education %}
<table class="responsive-table">
  <thead>
    <tr>
      <th>时间段</th>
      <th>院校</th>
      <th>专业</th>
      <th>学位</th>
    </tr>
  </thead>
  <tbody>
    {% for edu in educations %}
    <tr>
      <td data-label="period">{{ edu.period }}</td>
      <td data-label="university">
        <a href="{{ edu.university.url }}" target="_blank">
          {{ edu.university.name }}
        </a>
      </td>
      <td data-label="major">{{ edu.major }}</td>
      <td data-label="degree">{{ edu.degree }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>{% endraw %}

Work experience
======

|   Date    | Institution | Department | Position |
| :-------: | :---------: | :--------: | :------: |
| 2025.-Now |             |            |          |

Publications
======

  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Talks
======
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>

Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Service and leadership
======
