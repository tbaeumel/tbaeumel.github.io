---
layout: archive
title: "Selected publications"
permalink: /publications/
author_profile: true
---

You can find a complete list of my articles on <u><a href="https://scholar.google.com/citations?hl=de&user=y4OhikAAAAAJ">my Google Scholar profile</a>.</u>


{% include base_path %}

<div class="publications">
  {% assign pubs = site.publications | sort: "date" | reverse %}
  {% for pub in pubs %}
    <div class="publication-item" style="margin-bottom: 1.5em;">
      <strong>{{ pub.title }}</strong><br>
      <em>{{ pub.venue }}</em> ({{ pub.date | date: "%Y" }})<br>
      {% if pub.paperurl %}
        <a href="{{ pub.paperurl }}" target="_blank">View Paper</a>
      {% endif %}
      {% if pub.abstract %}
        <p style="margin-top: 0.5em;">{{ pub.abstract }}</p>
      {% endif %}
    </div>
  {% endfor %}
</div>