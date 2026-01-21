---
title: People
layout: single
collection: people
---

## Instructor

| Name                   |  Contact Address                                                   | Office Hours                   | Office Hours Location                   |
|------------------------|--------------------------------------------------------------------|--------------------------------|-----------------------------------------|
| {{ site.author.name }} |  [{{ site.author.emailaddr }}](mailto:{{ site.author.emailaddr }}) | {{ site.author.office_hours }} | {{ site.author.office_hours_location }} |

## TA Staff
Tutoring is ***free*** and will take place in Arts and Sciences 111.
![Path to Tutoring Room]( {{ site.baseurl }}/assets/images/classroom-to-tutoring-room.jpg)

|Name                                                       | Role              | Contact Address                               | Tutoring Hours            |
|-----------------------------------------------------------|-------------------|-----------------------------------------------|---------------------------|
{% for person in site.data.personnel %} | {{ person.name }} | {{ person.role }} | [{{ person.email }}](mailto:{{ person.email }}) | {{ person.office_hours }} |
{% endfor %}

![Logical Distortion]({{ site.baseurl }}/assets/images/aura-of-logical-distortion.gif "Sometimes it helps just having someone else around")