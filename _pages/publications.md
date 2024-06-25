---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

# Publications

{% for publication in site.publications %}
<div class="publication-item">
    <h2><a href="{{ publication.url }}">{{ publication.title }}</a></h2>
    <p><strong>{{ publication.venue }}</strong>, {{ publication.date | date: "%Y-%m-%d" }}</p>
    {% if publication.image %}
    <img src="{{ publication.image }}" alt="Image for {{ publication.title }}" style="max-width: 300px;">
    {% endif %}
    <p>{{ publication.excerpt }}</p>
    {% if publication.abstract %}
    <details>
      <summary>Abstract</summary>
      <p>{{ publication.abstract }}</p>
    </details>
    {% endif %}
</div>
<hr>
{% endfor %}