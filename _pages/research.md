
---
title: "Research"
layout: page
permalink: /research/
---

# Research

<div class="research-grid">

<div class="research-card">
<div class="research-image">
<img src="{{ '/images/research/white_plague.jpg' | relative_url }}" class="research-thumb" width="400" height="200" alt="white plague disease">
<p class="photo-attribution">Ernesto Weil, Caribbean Coral Reef Institute</p>
</div>
<div class="research-body">
<h2 class="research-title">Viruses Associated with White Plague Disease</h2>
<p class="research-desc">White plague is a tissue loss disease that affects many coral species and has contributed substantially to Caribbean reef decline. Although bacteria have been investigated as etiological agents, a consistent pathogen has not been identified. The role of viruses in white plague disease remains relatively unexplored, with the only study to date focused on DNA viruses. I use transcriptomics and transmission electron microscopy (TEM) to identify actively transcribed DNA and RNA viruses associated with white plague disease. Preliminary results suggest that viruses with sequence similarity to Betaflexiviridae, a family of plant-infecting filamentous single stranded RNA viruses (ssRNAVs) are overrepresented in white plague-affected tissue. Putative filamentous virus-like particles have been observed in Symbiodiniaceae, the coral’s micro-eukaryotic symbiotic partner, and are associated with damage to its chloroplasts. These findings suggest that infection by filamentous ssRNAVs may impair Symbiodiniaceae function and potentially contribute to white plague disease development in corals.</p>
</div>
</div>

<div class="research-card">
<div class="research-image">
<img src="{{ '/images/research/dinoRNAV.jpg' | relative_url }}" class="research-thumb" width="400" height="200" alt="dinoRNAV">
<p class="photo-attribution">Photo: [Photographer / source]</p>
</div>
<div class="research-body">
<h2 class="research-title">Prevalence and Impacts of dinoRNAV Infection in Symbiodniaceae</h2>
<p class="research-desc">Symbiodiniaceae-infecting positive-sense single-stranded RNA viruses (dinoRNAVs) have been reported in six genera of corals. Additionally, 93% of Porites lobata colonies on the north shore of Moorea, French Polynesia, show detectable dinoRNAV infection. While these viruses seem common, coral holobionts harbor millions of Symbiodiniaceae cells per square centimeter of tissue, and it remains unknown to what extent Symbiodiniaceae communities within coral colonies are infected. Additionally, while it has been hypothesized that dinoRNAVs may play a role in coral bleaching via Symbiodiniaceae lysis, the impact of dinoRNAV infection has not been experimentally explored. I plan to use single cell RNA sequencing to fill these gaps.</p>
</div>
</div>

<div class="research-card">
<div class="research-image">
<img src="{{ '/images/research/fermentation.png' | relative_url }}" class="research-thumb" width="400" height="200" alt="fermentation of traditional foods">
</div>
<div class="research-body">
<h2 class="research-title">Microbes Involved in the Fermention of Traditional Foods</h2>
<p class="research-desc">This is a side project which aims to answer community questions in Moorea, French Polynesia.</p>
<h2 class="publications">
</div>
</div>

</div>

<style>
.research-grid {
  display: flex;
  flex-direction: column;
  gap: 24px;
  width: 100%;
}

.research-card {
  display: flex;
  flex-direction: row;
  align-items: flex-start;
  gap: 24px;
  width: 100%;
}

.research-image {
  width: 250px;
  flex-shrink: 0;
}

.research-card .research-thumb {
  display: block;
  width: 250px;
  height: 250px;
  object-fit: cover;
}

.photo-attribution {
  font-size: 0.75rem;
  color: #777;
  margin: 6px 0 0;
  line-height: 1.4;
}

.research-card .research-body {
  flex: 1;
  min-width: 0;
}

@media (max-width: 700px) {
  .research-card {
    flex-direction: column;
  }

  .research-image {
    width: 100%;
  }

  .research-card .research-thumb {
    width: 100%;
    height: 250px;
    object-fit: cover;
  }
}
</style>
