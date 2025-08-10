---
permalink: /courses/
---

# Attended courses

## Master's programme in Mathematics

| Year | Course || Credits  |  
|------|--------||----------|{% for entry in site.data.taken_courses['master'] %}{% assign first = true %}{% for code in entry.courses %}
{% if first %}|**{{ entry.year }}** |{% assign first = false %}{% else %}| |{% endif %} {{code}}: {{ site.data.courses[code].name }}||{{ site.data.courses[code].credits }} ECTS|{% endfor %}{% endfor %}
| |  |Tot:|**120ECTS** |



## Bachelor's Programme in Computer Science

| Year | Course || Credits  |  
|------|--------||----------|{% for entry in site.data.taken_courses['bachelor'] %}{% assign first = true %}{% for code in entry.courses %}
{% if first %}|**{{ entry.year }}** |{% assign first = false %}{% else %}| |{% endif %} {{code}}: {{ site.data.courses[code].name }}||{{ site.data.courses[code].credits }} ECTS|{% endfor %}{% endfor %}
| |  |Tot:|**180 ECTS**|

## Additional courses

| Year | Course || Credits  |  
|------|--------||----------|{% for entry in site.data.taken_courses['other'] %}{% assign first = true %}{% for code in entry.courses %}
{% if first %}|**{{ entry.year }}** |{% assign first = false %}{% else %}| |{% endif %} {{code}}: {{ site.data.courses[code].name }}||{{ site.data.courses[code].credits }} ECTS|{% endfor %}{% endfor %}
| |  |Tot:|**52.5 ECTS**|
