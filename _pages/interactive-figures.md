---
title: "Animations and Interactive Figures"
permalink: /interactive-figures/
author_profile: true
---

<style>
.figure-item {
  border: 1px solid #e0e0e0;
  border-radius: 6px;
  padding: 1em 1.3em;
  margin-bottom: 1em;
  background: #fff;
}
.figure-item h3 { margin: 0 0 0.3em 0; font-size: 1em; }
.figure-item p { font-size: 0.93em; color: #444; margin: 0.3em 0 0.6em; line-height: 1.6; }
.figure-item .figure-meta { font-size: 0.85em; color: #888; margin-bottom: 0.5em; }
.figure-item .figure-links a { font-size: 0.9em; margin-right: 0.8em; }

details.anim-item {
  border: 1px solid #e0e0e0;
  border-radius: 6px;
  margin-bottom: 1em;
  background: #fff;
}

details.anim-item[open] {
  border-color: #bbb;
}

details.anim-item summary {
  padding: 0.85em 1.1em;
  cursor: pointer;
  font-size: 1em;
  font-weight: 600;
  list-style: none;
  display: flex;
  justify-content: space-between;
  align-items: center;
  user-select: none;
}

details.anim-item summary::-webkit-details-marker { display: none; }

details.anim-item summary::after {
  content: "▶ Play";
  font-size: 0.85em;
  color: #999;
  font-weight: 400;
}

details.anim-item[open] summary::after {
  content: "■ Stop";
}

.anim-content {
  padding: 0.5em 1.3em 1.3em;
  border-top: 1px solid #eee;
}

.anim-content p { font-size: 0.93em; color: #444; margin: 0.6em 0; line-height: 1.6; }
.anim-content .figure-meta { font-size: 0.85em; color: #888; margin-bottom: 0.6em; }
.anim-content .figure-links a { font-size: 0.9em; margin-right: 0.8em; }
</style>

## Animations

<details class="anim-item" id="vimes-animation">
  <summary>VIMES — Visualization of Massive Evolving Stars &nbsp;<span style="font-weight:400; font-size:0.85em; color:#888;">Laya Binu · 2025</span></summary>
  <div class="anim-content">
    <p class="figure-meta">Laya Binu (GW Paleontology Lab, UC San Diego) · <a href="https://github.com/layabinu/VIMES_VIsualization_of_Massive_Evolving_Stars" target="_blank">GitHub</a></p>
    <p>VIMES is an interactive visualization tool for massive evolving stars, developed by GW Paleontology group member Laya Binu. The tool provides animated visual representations of stellar evolution tracks and properties, making it easier to explore and communicate how massive stars evolve over their lifetimes.</p>
    <video id="vimes-video" width="100%" controls muted playsinline loop style="border-radius: 4px; margin-top: 0.5em; border: 1px solid #e0e0e0;">
      <source src="/files/videos/VIMES.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</details>

<script>
(function () {
  var details = document.getElementById('vimes-animation');
  var video   = document.getElementById('vimes-video');
  if (details && video) {
    details.addEventListener('toggle', function () {
      if (details.open) {
        video.currentTime = 0;
        video.play();
      } else {
        video.pause();
        video.currentTime = 0;
      }
    });
  }
})();
</script>

---

## Interactive Figures

<div class="figure-item">
  <h3>Formation Channel Rates — Interactive Catalog</h3>
  <p class="figure-meta">Broekgaarden et al. 2026 · <em>How Common Are Common Envelopes? Quantifying Their Role in Forming Gravitational-Wave Sources</em></p>
  <p>Interactive table and figures exploring the fractional contributions of formation channels (with and without common-envelope evolution) across 200+ population-synthesis simulations for binary black holes, BH–neutron star systems, and binary neutron stars. Includes sortable tables, parameter comparisons, and rate distributions.</p>
  <div class="figure-links">
    <a href="https://floorbroekgaarden.github.io/Rates_of_Formation_Channels/interactive_figures_and_tables/formation_channel_rates_table.html" target="_blank">Open interactive catalog</a>
    <a href="https://arxiv.org/abs/2606.05322" target="_blank">arXiv:2606.05322</a>
  </div>
</div>

<div class="figure-item">
  <h3>LOWER YOUR RATES — Interactive Figures and Tables</h3>
  <p class="figure-meta">Broekgaarden et al. · <em>On Claims of a Binary Black Hole Merger-Rate Crisis</em></p>
  <p>Interactive figures and tables for the LOWER YOUR RATES paper exploring binary black hole merger rate constraints and comparisons across different studies and methodologies.</p>
  <div class="figure-links">
    <a href="https://floorbroekgaarden.github.io/lower-your-rates/" target="_blank">Open interactive figures</a>
    <a href="https://zenodo.org/records/5072400" target="_blank">Zenodo: 10.5281/zenodo.5072400</a>
    <a href="https://github.com/FloorBroekgaarden/Rates_of_Compact_Object_Coalescence" target="_blank">GitHub</a>
  </div>
</div>
