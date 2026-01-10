---
layout: archive
title: "Education"
permalink: /education/
author_profile: true
---

{% include base_path %}

{% for ed in site.data.cv.education %}
### {{ ed.institution }}

{% if ed.studyType %}{{ ed.studyType }} {% endif %}{{ ed.area }}

{% if ed.startDate or ed.endDate %}
_{{ ed.startDate }}{% if ed.endDate %} — {{ ed.endDate }}{% endif %}_
{% endif %}

{% if ed.gpa %}
GPA: {{ ed.gpa }}
{% endif %}

{% if ed.courses and ed.courses.size > 0 %}
Courses:

{% for c in ed.courses %}
- {{ c.name }}
{% endfor %}

{% endif %}

{% endfor %}
