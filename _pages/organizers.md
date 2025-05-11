---
title: "Organizers"
layout: default
permalink: /organizers/
author_profile: false
---


<div class="organizers-grid">
  {% for org in site.data.organizers %}
    <div class="organizer-card">
      <img src="{{ org.image | default: '/assets/images/bio-photo.jpg' | relative_url }}"
           alt="{{ org.name }}"
           class="organizer-avatar" />
      <h3 class="organizer-name">{{ org.name }}</h3>
      <p class="organizer-role">{{ org.role }}</p>
      <p class="organizer-description">{{ org.description }}</p>
    </div>
  {% endfor %}
</div>

.