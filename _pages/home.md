---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero">{{ site.name }}</h1>
<p class="home-hero-sub">{{ site.title }}, {{ site.institution }}</p>

<div class="chip-container" markdown="0">
<a href="{{ '/research' | relative_url }}" class="chip">Coral Microbial Ecology</a>
<a href="{{ '/research' | relative_url }}" class="chip">Coral Disease</a>
<a href="{{ '/research' | relative_url }}" class="chip">Virologyy</a>
</div>

I am interested in the role of viruses in coral health and disease. Viruses are the most abundant and diverse biological entities on Earth! They infect everything, from humans to bacteria. Corals host a wide diversity of micro-organisms including bacteria, fungi and micro-eukaryotes like Symbiodiniaceae. Some of these microorganisms play key roles in coral health. For example, through photosynthesis, Symbiodiniaceae provide the majority of coral’s energy. Viruses can infect the coral animal as well as their microbes. I am interested in whether viral infection of these mutualist microbes can reduce their function and lead to coral health decline.

{% comment %}
<div class="callout callout-success" markdown="0">
<div class="callout-title">{% include icon.html name="award" class="callout-icon" %} Nobel Prize in Physics, 1965</div>
<p>Awarded the Nobel Prize jointly with Julian Schwinger and Shin'ichiro Tomonaga for fundamental work in quantum electrodynamics, with deep-ploughing consequences for the physics of elementary particles.</p>
</div>
{% endcomment %}

<div class="banner-frame" markdown="0">
<img src="{{ '/images/banner.webp' | relative_url }}" alt="Feynman diagrams" width="1400" height="449" loading="lazy">
<div class="banner-caption">Viral infection of Symbiodiniaceae by Betaflexiviridae, a family of filamentous single stranded RNA viruses, may lead to white plague disease development (Sookhoo et al., in prep). Viral relpication dinoRNAVs, a group of icosahedral single stranded RNA viruses, that infect Symbiodiniaceae is triggered by heat stress and may contribute to coral bleaching (Howe-Kerr et al., 2023)</div>
</div>

{% comment %}
{% capture selected %}{% bibliography --query @*[selected=true] %}{% endcapture %}
{% if selected contains "pub-entry" %}
## Selected publications

<div class="section-card selected-pubs" markdown="0">
{{ selected }}
<p style="margin: var(--space-4) 0 0;"><a href="{{ '/publications' | relative_url }}">All publications &rarr;</a></p>
</div>
{% endif %}
{% endcomment %}

## About me

I was born and grew up in Trinidad and Tobago, two small islands in the Caribbean. At seven years old, I decided that I wanted to be a marine biologist because I wanted to go to the beach everyday. Today, I'm a graduate student in Collaboration for Ocean Futures lab at UC Berkeley, where I study the role of microbes in coral health.

Outside of work, I am learning French; je suis le cours de français 3. I like to read fantasy, sci-fi and dystopia, cuddle with Potato (my roommate's cat), and watch crappy TV.
