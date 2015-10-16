---
layout: page
title: Members
description: Regular Attendees of OpenHack Syracuse
---
{% for member in site.data.members %}
## {{member.name}}

<img src="{{member.img}}" style="float: left; height: 160px; margin-right: 20px;" />

{% if member.social.twitter %}
<i class="fa fa-twitter"></i> [{{member.social.twitter}}](//twitter.com/{{member.social.twitter}})
{% endif %}
{% if member.social.website %}
<i class="fa fa-globe"></i> [{{member.social.website}}](//twitter.com/{{member.social.website}})
{% endif %}
{% if member.social.email %}
<i class="fa fa-envelope"></i> [{{member.social.email}}](//twitter.com/{{member.social.email}})
{% endif %}
{{member.desc | truncate: 100 }}
{% endfor %}
