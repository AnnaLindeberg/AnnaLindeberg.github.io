---
permalink: /teaching/
---
# Teaching

In the following table, you will find a full breakdown of courses I've taught in.
All courses are at Bachelor's level given at Stockholm University, except where indicated.
I worked approximately 660
hours with teaching at SU during 2020--2023, and around 280 hours at LiU in 2022.
Teaching as part of my PhD position constitutes 20% full-time or,
approximately, 400 hours per year.

| Semester      | Course Code | Course Name                                         |
|---------------|-------------|-----------------------------------------------------|{% for entry in site.data.teaching %}{% assign first = true %}{% for code in entry.courses %}
{% if first %}|**{{ entry.semester }}** |{% assign first = false %}{% else %}| |{% endif %}[{{code}}]({{site.data.courses[code].url}}) {% if site.data.courses[code].note %}[^{{site.data.courses[code].note}}]{% endif %} | {{ site.data.courses[code].name }}|{% endfor %}{% endfor %}

{% for noteid in site.data.course_notes %}
[^{{noteid[0]}}]: {{noteid[1]}}
{% endfor%}