---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

<style>
.research-intro { font-size: 0.97em; margin-bottom: 2em; line-height: 1.6; }
.research-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1.8em;
  margin-top: 1em;
}
@media (max-width: 640px) {
  .research-grid { grid-template-columns: 1fr; }
}
.research-tile {
  border: 1px solid #e5e5e5;
  border-radius: 6px;
  overflow: hidden;
  background: #fff;
}
.research-tile img {
  width: 100%;
  height: 180px;
  object-fit: cover;
  display: block;
}
.research-tile-placeholder {
  width: 100%;
  height: 180px;
  background: #e8e8e8;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #aaa;
  font-size: 0.8em;
}
.research-tile-body {
  padding: 0.8em 1em 1em;
}
.research-tile-body h3 {
  margin: 0 0 0.5em;
  font-size: 0.95em;
  line-height: 1.4;
  color: #222;
}
.research-tile-body p {
  margin: 0;
  font-size: 0.88em;
  color: #555;
  line-height: 1.55;
}
</style>

<p class="research-intro">My research focuses on <strong>Gravitational Wave Paleontology</strong> — using observations of merging black holes and neutron stars to study the evolutionary history of massive stars. A central challenge is the <em>Progenitor Uncertainty Challenge</em>: understanding and managing the large theoretical uncertainties in stellar evolution models so that gravitational-wave data can be used to extract meaningful astrophysical insights. My work spans stellar evolution simulations, statistical and machine-learning methods, population synthesis, and open-science infrastructure.</p>

<div class="research-grid">

  <div class="research-tile">
    <img src="/images/research_compas.png" alt="Simulating stars">
    <div class="research-tile-body">
      <h3>Simulating billions of stars and the black holes &amp; neutron stars they form</h3>
      <p>I use rapid population synthesis codes — primarily <a href="https://compas.science">COMPAS</a> — to simulate large grids of binary star systems and model how massive stars evolve into black holes and neutron stars. Running millions of simulations across diverse physical assumptions lets me map the vast uncertainty space in stellar evolution theory and generate theoretical merger populations to compare with gravitational-wave observations.</p>
    </div>
  </div>

  <div class="research-tile">
    <div class="research-tile-placeholder">image coming soon</div>
    <div class="research-tile-body">
      <h3>Investigating the cosmic star formation history using gravitational waves</h3>
      <p>The redshift distribution of gravitational-wave merger events encodes how star formation has evolved across cosmic time. By comparing observed merger rates with theoretical models tied to the star formation history, I work to reconstruct how the conditions for forming merging compact binaries have changed over billions of years of cosmic evolution.</p>
    </div>
  </div>

  <div class="research-tile">
    <img src="/images/research_gwdetectors.png" alt="Future GW detectors">
    <div class="research-tile-body">
      <h3>Future gravitational wave detectors</h3>
      <p>Next-generation observatories such as the <a href="https://www.et-gw.eu/">Einstein Telescope</a> and <a href="https://cosmicexplorer.org/">Cosmic Explorer</a> will detect hundreds of thousands of compact binary mergers per year — orders of magnitude more than current detectors. I study what astrophysical science these instruments will enable and help prepare the theoretical models and analysis frameworks needed to fully exploit their data.</p>
    </div>
  </div>

  <div class="research-tile">
    <div class="research-tile-placeholder">image coming soon</div>
    <div class="research-tile-body">
      <h3>Investigating the lives of binary stars</h3>
      <p>Most massive stars live in binary systems, and the evolutionary interactions between companions — mass transfer, common envelope evolution, stellar winds, and supernova kicks — largely determine whether a binary produces a merging pair of compact objects. Gravitational-wave observations offer a new, independent way to constrain these poorly understood phases of binary stellar evolution.</p>
    </div>
  </div>

  <div class="research-tile">
    <div class="research-tile-placeholder">image coming soon</div>
    <div class="research-tile-body">
      <h3>Developing statistical, AI, and ML techniques for stellar populations &amp; gravitational waves</h3>
      <p>Connecting large gravitational-wave catalogs to high-dimensional population synthesis models requires new computational tools. I develop Bayesian hierarchical inference methods, emulators, and machine-learning approaches that make it tractable to explore the full parameter space of stellar evolution models and rigorously quantify the uncertainties in astrophysical population analyses.</p>
    </div>
  </div>

  <div class="research-tile">
    <div class="research-tile-placeholder">image coming soon</div>
    <div class="research-tile-body">
      <h3>Supporting software, big and open data, and reproducibility/transparency in science</h3>
      <p>Reproducibility and open science are central to my research practice. I contribute to open-source tools including the <a href="https://www.tomwagg.com/software-citation-station/">Software Citation Station</a>, advocate for public data releases alongside publications, and work to make population synthesis grids and analysis pipelines openly accessible so that results can be independently verified and built upon.</p>
    </div>
  </div>

</div>
