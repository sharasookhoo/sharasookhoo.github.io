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
<img src="{{ '/images/' | append: article.image | relative_url }}" class="research-thumb" alt="{{ article.headline }}" loading="lazy">
{% endif %}

<div class="research-body">
<span class="news-date">{{ article.date }}</span>
<h2 class="research-title">{{ article.headline }}</h2>
</div>

</div>

{% endfor %}

</div>

<style>
.research-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 24px;
  width: 100%;
}

.research-card {
  display: flex;
  flex-direction: column;
  overflow: hidden;
}

.research-card .research-thumb {
  width: 100%;
  aspect-ratio: 1 / 1;
  height: auto;
  object-fit: cover;
  display: block;
}

.research-body {
  padding: 16px;
}

.news-date {
  display: block;
  font-size: 0.8rem;
  color: #777;
  margin-bottom: 8px;
}

.research-title {
  font-size: 1.1rem;
  line-height: 1.4;
}

@media (max-width: 900px) {
  .research-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }
}

@media (max-width: 600px) {
  .research-grid {
    grid-template-columns: 1fr;
  }
}
</style>
