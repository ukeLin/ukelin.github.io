---
permalink: /
title: "Chunlin Yu"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Ph.D. student in Computer Science and Technology at **University of Science and Technology Beijing**. My research lies in computer vision and medical image analysis, with a focus on designing efficient architectures for biomedical imaging.

News
======
- **[08/2026]** One paper accepted by **TNNLS**.
- **[08/2026]** One paper accepted by **ESWA**.

Research Interests
======
- Computer Vision
- Medical Image Analysis

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
    </div>
  </div>
{% endfor %}
</div>
