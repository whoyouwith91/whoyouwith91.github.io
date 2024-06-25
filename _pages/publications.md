---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% for publication in site.publications %}
1. [{{ publication.title }}]({{ publication.url }})
   *{{ publication.venue }}*, {{ publication.date | date: "%Y-%m-%d" }}
{% endfor %}
