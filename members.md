---
layout: page
title: Members
description: Regular Attendees of OpenHack Syracuse
---

{% for member in site.data.members offset: 1 %}
### {{member.name}}
{% if member.social.twitter %}
- Twitter: [{{member.social.twitter}}](//twitter.com/{{member.social.twitter}})
{% end %}
{% if member.social.website %}
- Website: [{{member.social.website}}](//twitter.com/{{member.social.website}})
{% end %}
{{member.desc}}
<nr/>
{% endfor %}
