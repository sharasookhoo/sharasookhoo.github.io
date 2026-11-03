---
title: "About"
layout: page
permalink: /about/
---

# About

<!-- Panel 1: Photo and biography -->
<div class="section-card">
  <div class="pi-card">
    <img src="{{ site.photo | prepend: '/images/' | relative_url }}" class="pi-photo" alt="{{ site.name }}" width="160" height="160">
    <div>
      <h2 class="pi-name">{{ site.name }}</h2>
      I was born and grew up in Trinidad and Tobago, two small islands in the Caribbean. At seven years old, I decided that I wanted to be a marine biologist because I wanted to go to the beach everyday. As I learnt more about the importance of coral reefs as well as the significant challenges facing these ecosystems, my childhood dream matured into a desire to protect and restore corals. I pursued a B.S. in Marine Biology and Ecology, and a second major in Biochemistry and Molecular Biology at the University of Miami. During this time I worked in several labs including Mote's Coral Health and Disease lab in the Florida Keys and the Cnidarian Immunity lab at the Rosenstiel School of Marine, Atmospheric, and Earth Science. There, I was introduced to the fascinating world of coral microbes. I am currently a PhD candidate in the Collaboration for Ocean Futures Lab (COSL) led by Adrienne Correa at University of California, Berkeley where I investigate the role of viruses in coral health.
    </div>
  </div>
</div>

<!-- Panel 2: Research Experience -->
{% if site.data.research_experience %}
<div class="section-card">
  <h3>Research Experience</h3>
  <ul class="awards-list">
    {% for experience in site.data.research_experience %}
    <li>
      <strong>{{ experience.name }}</strong> <em>({{ experience.date }})</em>
      {% if experience.description %}
      <div class="award-description">{{ experience.description }}</div>
      {% endif %}
    </li>
    {% endfor %}
  </ul>
</div>
{% endif %}

<!-- Panel 3: Awards -->
{% if site.data.awards %}
<div class="section-card">
  <h3>Awards</h3>
  <ul class="awards-list">
    {% for award in site.data.awards %}
    <li>
      <strong>{{ award.name | replace: "-","&#8211;" }}</strong>{% if award.description %}, {{ award.description }}{% endif %} <em>({{ award.date }})</em>
    </li>
    {% endfor %}
  </ul>
</div>
{% endif %}

<!-- Panel 4: Leadership and Service -->
{% if site.data.mentorship_service %}
<div class="section-card">
  <h3>Leadership and Service</h3>
  <ul class="awards-list">
    {% for item in site.data.mentorship_service %}
    <li>
      <strong>{{ item.name }}</strong> <em>({{ item.date }})</em>
      {% if item.description %}
      <div class="award-description">{{ item.description }}</div>
      {% endif %}
    </li>
    {% endfor %}
  </ul>
</div>
{% endif %}

<style>
.section-card {
  width: 100%;
  box-sizing: border-box;
  margin-bottom: 24px;
}

.pi-card {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  gap: 24px;
}

.pi-photo {
  width: 160px;
  height: 160px;
  object-fit: cover;
  flex-shrink: 0;
}

.pi-card > div {
  flex: 1;
  min-width: 0;
}

.awards-list li {
  margin-bottom: 12px;
}

.award-description {
  margin-left: 1.5em;
  margin-top: 2px;
}

@media (max-width: 600px) {
  .pi-card {
    flex-direction: column;
  }
}
</style>
