
---
title: "News"
layout: page
permalink: /allnews.html
---

# News

<div class="research-grid">

{% for article in site.data.news %}
<div class="research-card">
  {% if article.image %}
  <img src="{{ '/images/' | append: article.image | relative_url }}"
       class="news-thumb"
       alt="{{ article.headline }}"
       loading="lazy">
  {% endif %}
  <div class="research-body">
    <span class="news-date">{{ article.date }}</span>
    <h2 class="research-title">{{ article.headline }}</h2>
  </div>
</div>
{% endfor %}

</div>

<style>
.news-thumb {
  width: 100%;
  aspect-ratio: 1 / 1;
  object-fit: cover;
  display: block;
}

@media (max-width: 700px) {
  .research-grid {
    grid-template-columns: 1fr;
  }
}
</style>
