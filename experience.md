---
title: Experience
permalink: /experience/
eyebrow: Career
hide_title: true
intro: From computer-vision research to building and deploying genAI.
---

<div class="timeline">
  {% for item in site.data.experience %}
  <section class="timeline-item">
    <div class="timeline-meta">
      <p>{{ item.period }}</p>
      <p>{{ item.location }}</p>
    </div>
    <div class="timeline-main">
      <p class="company">{{ item.company }}</p>
      <h2>{{ item.role }}</h2>
      <p>{{ item.summary }}</p>
    </div>
  </section>
  {% endfor %}
</div>
