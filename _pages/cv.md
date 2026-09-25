---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* **Ph.D. in Computer Science and Technology**, University of Science and Technology Beijing, 2025.09 – present
* **M.S. in Computer Science and Technology**, Liaoning Technical University, 2022.09 – 2025.06
* **B.S. in Computer Science and Technology**, Liaoning Technical University, 2018.09 – 2022.06

Publications
======
<div class="pub-list">
{% assign sorted_pubs = site.publications | sort: "date" | reverse %}
{% for post in sorted_pubs %}
  <div class="pub-item">
    <div class="pub-title">
      <a href="{{ post.paperurl }}" target="_blank" rel="noopener">{{ post.title }}</a>
    </div>
    <div class="pub-authors">
      {{ post.authors | replace: "Chunlin Yu", "<strong>Chunlin Yu</strong>" | replace: "<strong><strong>Chunlin Yu</strong></strong>", "<strong>Chunlin Yu</strong>" }}
    </div>
    <div class="pub-venue">
      <em>{{ post.venue }}</em>, {{ post.year }}.
      {% if post.volume %} <span class="pub-vol">{{ post.volume }}.</span>{% endif %}
    </div>
  </div>
{% endfor %}
</div>
