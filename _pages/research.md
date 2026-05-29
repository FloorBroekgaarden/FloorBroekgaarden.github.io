---
layout: archive
title: "Gravitational Wave Paleontology Group Research"
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

<video autoplay loop muted playsinline style="width: 100%; max-width: 860px; border-radius: 6px; margin-bottom: 1.5em; display: block;">
  <source src="/files/videos/GW_video_merger.mp4" type="video/mp4">
</video>

<div style="background: #f7f7f7; border-left: 4px solid #555; padding: 1em 1.4em; margin-bottom: 2em; max-width: 860px; border-radius: 0 4px 4px 0;">
<p style="margin: 0; font-size: 0.97em; line-height: 1.75; font-style: italic;"><strong>Mission:</strong> Our mission is to open and lead the new frontier of gravitational-wave paleontology: reconstructing the history of massive stars and compact objects across cosmic time using gravitational waves as cosmic fossils. We seek to transform gravitational-wave astronomy from the discovery of individual events into a precision population science capable of revealing how massive stars form, evolve, interact, explode, and shape the Universe. By combining astrophysics, AI, statistics, and large-scale computation, our group develops the tools, simulation ecosystems, and uncertainty-aware frameworks needed to connect gravitational-wave observations back to their progenitor stars and tackle the fundamental "simulation silo" challenge in stellar evolution. Through interdisciplinary, student-driven research and a strong commitment to open and collaborative science, we aim to build a new framework for understanding the dynamic Universe; from the first generations of stars to the black holes and neutron stars merging today.</p>
</div>

<div style="font-size: 0.97em; line-height: 1.75; margin-bottom: 2em; max-width: 860px;">

<p>The Gravitational-Wave Paleontology Group studies the formation, lives, and explosive deaths of massive stars across cosmic time using gravitational waves as "cosmic fossils." When black holes and neutron stars merge, they produce ripples in spacetime that carry information about the stars that formed them billions of years earlier. By studying these mergers, we aim to answer some of the biggest open questions in astrophysics today: How do black holes and neutron stars form? Which evolutionary pathways produce the gravitational-wave sources we observe? And what can these mergers teach us about the lives, environments, and deaths of massive stars throughout the history of the Universe? This emerging field — gravitational-wave paleontology — opens an entirely new way of studying stellar evolution, allowing us to probe populations of massive stars that are otherwise inaccessible to traditional light-based astronomy because they lived in the distant, early Universe or died long ago.</p>

<p>We are entering the Big Data era of gravitational-wave astronomy. Over the next decade, detectors such as LIGO, Virgo, Cosmic Explorer, the Einstein Telescope, and LISA will increase the number of observed compact-object mergers from hundreds today to millions per year, extending observations to the edge of the observable Universe. However, interpreting this wealth of data requires overcoming a major challenge: gravitational waves do not directly reveal the properties of the progenitor stars that formed them. Instead, connecting observations back to stellar evolution requires large-scale theoretical simulations that model how massive binaries evolve over billions of years. At present, these simulations are computationally expensive, highly uncertain, and often fragmented into isolated "simulation silos," where different groups explore only narrow regions of parameter space within individual codes. These silos obscure uncertainties, bias physical interpretation, and limit our ability to learn robustly from gravitational-wave observations.</p>

<p>Our group tackles this challenge by combining astrophysics, AI/ML, statistics, and scientific computing to build new uncertainty-aware frameworks, simulation catalogs, and data-driven tools that can transform gravitational-wave detections into a quantitative fossil record of massive-star evolution across cosmic time. Central to this effort is the development of <strong>GROWL</strong> (<em>GRavitatiOnal Wave paLeontology</em>), a next-generation, community-driven simulation ecosystem that will unify thousands of simulations across formation channels, stellar evolution codes, and physical assumptions into a single interoperable framework. By breaking today's fragmented "simulation silos," GROWL aims to make it possible, for the first time, to robustly connect observed gravitational-wave populations back to their progenitor stars and directly test which physical processes — such as mass transfer, supernovae, stellar winds, metallicity, and dynamical interactions — shape the black holes and neutron stars we observe across the Universe. Through this framework, our group seeks to answer some of the defining questions of modern astrophysics: How do gravitational-wave sources form? How did massive stars live and die in the early Universe? And what can black hole and neutron star mergers reveal about the cosmic history of stars, galaxies, and chemical enrichment?</p>

<p>Our research spans scales from the interiors of massive stars to the evolution of galaxies across cosmic time. We develop large-scale gravitational-wave simulation catalogs, AI-driven statistical emulators, interactive visualization tools, and next-generation inference frameworks capable of exploring the enormous uncertainty landscape of stellar evolution. The group investigates some of the most uncertain and influential processes in astrophysics — including mass transfer, common envelope evolution, stellar winds, supernova explosions, compact-object formation, and chemical enrichment — while connecting gravitational-wave populations to electromagnetic observations across the multi-messenger Universe. Our projects range from black hole population synthesis, cosmological enrichment histories, and kilonova modeling to the science case of future observatories such as Cosmic Explorer, the Einstein Telescope, and LISA.</p>

<p>The lab is deeply interdisciplinary and student-driven, bringing together researchers from astrophysics, data science, statistics, AI/ML, and scientific computing to develop both new scientific insight and new computational methodologies. Students in the group work at the frontier of gravitational-wave astronomy while gaining experience in high-performance computing, machine learning, visualization, statistical inference, and open-source scientific software development. By combining theory, computation, machine learning, and multi-messenger astrophysics, the lab aims not only to advance gravitational-wave astronomy, but to establish gravitational-wave paleontology as a foundational new frontier for understanding how massive stars shaped the Universe across cosmic history.</p>

</div>

<hr style="margin-bottom: 2em;">


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
