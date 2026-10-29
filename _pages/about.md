---
permalink: /
title: "Chunlin Yu"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<div class="home-intro">
  <p>I am a Ph.D. student at the University of Science and Technology Beijing. My research interests include computer vision, medical image analysis, and foundation models.</p>
  <div class="home-interests" aria-label="Research interests">
    <span>Computer Vision</span><span>Medical Image Analysis</span><span>Foundation Models</span>
  </div>
</div>

## News

<div class="home-news">
  <div class="home-news__item"><time datetime="2026-10">Oct 2026</time><span>Selected for the inaugural cohort of the China Association for Science and Technology (CAST) Youth Talent Support Program for Doctoral Students.</span></div>
  <div class="home-news__item"><time datetime="2026-10">Oct 2026</time><span>Received the National Scholarship.</span></div>
  <div class="home-news__item"><time datetime="2026-08">Aug 2026</time><span>One paper accepted by <strong>TNNLS</strong>.</span></div>
  <div class="home-news__item"><time datetime="2026-08">Aug 2026</time><span>One paper accepted by <strong>ESWA</strong>.</span></div>
</div>

## Honors and Awards

<div class="home-news">
  <div class="home-news__item"><time datetime="2026">2026</time><span>Inaugural cohort, China Association for Science and Technology (CAST) Youth Talent Support Program for Doctoral Students</span></div>
  <div class="home-news__item"><time datetime="2026">2026</time><span>National Scholarship</span></div>
</div>

## Publications
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
      {% if post.impact_factor_2025 %}<span class="pub-metrics">IF {{ post.impact_factor_2025 }}</span>{% endif %}
    </div>
  </div>
{% endfor %}
</div>
