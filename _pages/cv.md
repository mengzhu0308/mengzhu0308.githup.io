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

```
{% raw %}{% assign educations = site.data.education %}

<div class="table-wrapper">
  <table>
    <thead>
      <tr>
        <th>Period</th>
        <th>University</th>
        <th>Major</th>
        <th>Degree</th>
      </tr>
    </thead>
    <tbody>
      {% for edu in educations %}
      <tr>
        <td>{{ edu.period }}</td>
        <td>
          <a href="{{ edu.university.url }}" target="_blank" rel="noopener">
            {{ edu.university.name }}
          </a>
        </td>
        <td>{{ edu.major }}</td>
        <td>{{ edu.degree }}</td>
      </tr>
      {% endfor %}
    </tbody>
  </table>
</div>{% endraw %}
```



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
