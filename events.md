---
layout: page
title: Events
description: Upcoming and Past OpenHack Meetups
header-img: "img/coworks-bg.jpg"
---

{% include next_meetup.html %}


### Previous meetups
{% for event in site.data.events offset: 1 %}
- {{ event.date | date: "%a, %B %d, %Y at %-I:%M%p" }} at {% if event.location == 'ttg' %}The Tech Garden{% elsif event.location == 'coworks' %}Syracuse Coworks{% endif %} {% if event.rsvp_link %} <a href='{{ event.rsvp_link }}'>RSVP Info</a> {% else %} (canceled) {% endif %}
{% endfor %}
