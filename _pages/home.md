---
title: "Home"
layout: homelay
permalink: /
---

<h1 class="home-hero">{{ site.name }}</h1>
<p class="home-hero-sub">{{ site.title }}, {{ site.institution }}</p>

<div class="chip-container" markdown="0">
<span class="chip">Coral Microbial Ecology</span>
<span class="chip">Coral Disease</span>
<span class="chip">Virology</span>
</div>

I am interested in the role of viruses in coral health and disease. Viruses are the most abundant and diverse biological entities on Earth! They infect everything, from humans to bacteria. Corals host a wide diversity of micro-organisms including bacteria, fungi and micro-eukaryotes like Symbiodiniaceae. Some of these microorganisms play key roles in coral health. For example, through photosynthesis, Symbiodiniaceae provide the majority of coral's energy. Viruses can infect the coral animal as well as their microbes. I am interested in whether viral infection of mutualistic microbes can lead to a loss of function and a reduction in host health.

<div class="banner-frame" markdown="0">
<img src="{{ '/images/banner.webp' | relative_url }}" alt="Feynman diagrams" width="1400" height="449" loading="lazy">
<div class="banner-caption">Viral infection of Symbiodiniaceae by Betaflexiviridae, a family of filamentous single stranded RNA viruses, may lead to white plague disease development (Sookhoo et al., in prep). Viral relpication dinoRNAVs, a group of icosahedral single stranded RNA viruses, that infect Symbiodiniaceae is triggered by heat stress and may contribute to coral bleaching (Howe-Kerr et al., 2023)</div>
</div>

#{% capture selected %}{% bibliography --query @*[selected=true] %}{% endcapture %}
#{% if selected contains "pub-entry" %}
## Selected publications

#<div class="section-card selected-pubs" markdown="0">
#{{ selected }}
#<p style="margin: var(--space-4) 0 0;"><a href="{{ '/publications' | relative_url }}">All publications &rarr;</a></p>
#</div>
#{% endif %}

