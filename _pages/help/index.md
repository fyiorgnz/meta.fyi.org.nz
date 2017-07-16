---
layout: page
title: FYI.org.nz Help Pages
permalink: /help/
---

{% for page in site.pages %} {% if page.tags contains "helppage" %}{% if page.title %}
 * <a href="{{ page.url | prepend: site.baseurl }}">{{ page.title }}</a>
{% endif %} {% endif %} {% endfor %}

