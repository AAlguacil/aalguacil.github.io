---
layout: page
title: Contact
permalink: /contact
---

Get in touch: <a href="mailto:antonio.alguacil.cabrerizo@usherbrooke.ca">antonio.alguacil.cabrerizo@usherbrooke.ca

You can also find me on social media:

{% for item in site.data.settings.social %}
  {% assign first_char = item.link | slice: 0 %}
  {% if first_char == '/' %}
    <a href="{{ site.baseurl }}{{ item.link }}"><i class="fa fa-{{ item.icon }} fa-2xl" aria-hidden="true"></i></a>
  {% else %}
    <a href="{{ item.link }}" target="_blank"><i class="fa fa-{{ item.icon }} fa-2xl" aria-hidden="true"></i></a>
  {% endif %}
{% endfor %}
