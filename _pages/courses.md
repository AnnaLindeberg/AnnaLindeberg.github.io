---
permalink: /courses/
---

# Attended courses

## Courses during PhD studies
In Sweden, there's a rather high requirement of courses taken during your time as a PhD student; I will need 60 ECTS.


| Term | Course | Credits  |  
|------|--------|----------|
| Spring 2025 | Research ethics | 1.5 ECTS |
| | Matroid Theory | 7.5 ECTS|
| | Topics in network science and graph theory | 5 ECTS |
| Fall 2024 | Introduction to teaching | 3 ECTS|
| | Soft skills for mathematicians | 5 ECTS|
|Summer 2024 | Czech Summer School of Combinatorics: Twin-width and contraction sequences | 1.5 ECTS|



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
