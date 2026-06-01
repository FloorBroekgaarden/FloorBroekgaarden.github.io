---
layout: archive
title: "Research Blog"
permalink: /research-blog/
author_profile: true
---

<style>
.blog-intro { font-size: 0.97em; line-height: 1.7; max-width: 780px; margin-bottom: 2em; }

details {
  border: 1px solid #e0e0e0;
  border-radius: 6px;
  margin-bottom: 0.8em;
  background: #fff;
}

details[open] {
  border-color: #bbb;
}

summary {
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

summary::-webkit-details-marker { display: none; }

summary::after {
  content: "＋";
  font-size: 1.1em;
  color: #999;
  font-weight: 300;
}

details[open] summary::after {
  content: "－";
}

.details-content {
  padding: 0.5em 1.4em 1.4em;
  border-top: 1px solid #eee;
  font-size: 0.95em;
  line-height: 1.75;
}

.details-content p { margin: 0.7em 0 0.9em; }

.item-date {
  font-weight: 400;
  font-size: 0.85em;
  color: #888;
  margin-left: 0.8em;
}

/* Blog post styles */
.details-content h2 {
  border-bottom: 1px solid #ddd;
  padding-bottom: 0.3em;
  margin: 2em 0 0.8em;
  font-size: 1.2em;
}

.details-content h3 {
  margin: 1.5em 0 0.5em;
  font-size: 1.05em;
}

.fig-block {
  margin: 1.5em 0;
  text-align: center;
}

.fig-block img {
  max-width: 100%;
  border: 1px solid #e8e8e8;
  border-radius: 4px;
}

.fig-caption {
  font-size: 0.85em;
  color: #555;
  margin-top: 0.4em;
  text-align: left;
  font-style: italic;
  max-width: 700px;
  margin-left: auto;
  margin-right: auto;
}

.highlight-box {
  background: #f5f8ff;
  border-left: 3px solid #5b8dd9;
  padding: 0.7em 1.1em;
  margin: 1.2em 0;
  border-radius: 2px;
  font-size: 0.93em;
}

.question-box {
  background: #fafafa;
  border-left: 3px solid #aaa;
  padding: 0.6em 1em;
  margin: 1em 0;
  border-radius: 2px;
  font-size: 0.92em;
}

.question-box .q-label {
  font-weight: bold;
  color: #555;
  font-size: 0.88em;
  text-transform: uppercase;
  letter-spacing: 0.04em;
}

.event-card {
  background: #f9f9f9;
  border: 1px solid #e5e5e5;
  border-radius: 5px;
  padding: 0.7em 1.1em;
  margin: 1em 0;
}

.event-card .event-name {
  font-family: monospace;
  font-size: 0.95em;
  font-weight: bold;
  color: #333;
}

.caveat {
  font-size: 0.87em;
  color: #666;
  border-top: 1px dashed #ddd;
  padding-top: 0.6em;
  margin-top: 1.5em;
}
</style>

<p class="blog-intro">Short posts, paper summaries, and research updates from the GW Paleontology Lab — covering both results from our group and highlights from the broader gravitational-wave and stellar astrophysics community. Meant as a resource for anyone wanting to stay up to date on the latest in gravitational-wave paleontology. Click any entry to expand it.</p>

<details>
  <summary>GWTC-5: My Summary of the New Gravitational-Wave Catalog <span class="item-date">May 29, 2026</span></summary>
  <div class="details-content">

<p><em>This is my astrophysics-focused summary of the new GWTC-5 gravitational-wave catalog papers released by the LIGO–Virgo–KAGRA (LVK) collaboration. It is a biased summary: I come at this from the angle of trying to use gravitational-wave data to understand the lives of massive stars, and the results I find most exciting reflect that. I gave a talk on this for the group this week; some of the thoughts below are drawn from that discussion.</em></p>

<h2>Part I: What is GWTC-5?</h2>

<p>GWTC-5 was released earlier this week — a suite of at least eight papers plus a new catalog. In a sentence: LVK has announced their gravitational-wave detections from the second half of their fourth observing run (O4b), analyzed the full combined dataset, and released a range of scientific results built on those detections.</p>

<p>Three things happened simultaneously:</p>
<ol>
  <li>LVK published the new <strong>individual compact-binary merger detections</strong> from O4b, including estimated source properties (masses, spins, distances).</li>
  <li>These are added to previous detections from O1, O2, O3, and O4a, forming <strong>GWTC-5</strong> — the fifth gravitational-wave transient catalog, with over 390 candidates in total.</li>
  <li>Using this expanded dataset, LVK analyzed <strong>population properties</strong>, cosmological constraints, tests of general relativity, and lensing signatures — each as a separate companion paper.</li>
</ol>

<p>One thing I love about this release is the video below, originally shared by Gabriele Vajente. It shows the growth of the "stellar graveyard" — a visualization of the masses of all compact objects detected with gravitational waves, accumulating over time from O1 through O4b. It really drives home how rapidly this field is growing.</p>

<div class="fig-block">
  <video controls style="max-width:100%; border-radius:4px; border:1px solid #e0e0e0;">
    <source src="/files/news/GWTC-5/1779814528172.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
  <div class="fig-caption">The growing stellar graveyard: gravitational-wave detections from O1 through O4b, visualized by mass. Orange dots are neutron stars, blue dots are black holes. The graveyard has grown from ~3 events in 2015 to over 390 candidates today. <em>Credit: Gabriele Vajente.</em></div>
</div>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot-2026-05-29-at-9.07.25-AM.png" alt="Timeline of LVK observing runs O1 through O4b">
  <div class="fig-caption"><strong>Figure 1</strong> from the Intro paper (<a href="https://arxiv.org/abs/2605.27223">arXiv:2605.27223</a>): Timeline of observing runs from 2015 through the beginning of O4c. Note that Virgo was absent for O4a but returned for O4b, significantly improving sky localization.</div>
</div>

<div class="question-box">
  <div class="q-label">A question that comes up</div>
  Why is the run now split into O4a, O4b, O4c — when earlier runs were just O1, O2, O3? The runs are getting longer, and the collaboration takes periodic maintenance breaks. These breaks are used to fix things, improve sensitivity, and calibrate. There's also a data-analysis reason: understanding noise well enough for rigorous parameter estimation is iterative and often improves after a run ends.
</div>

<p>The catalog now contains <strong>391 events</strong>. When I started working in gravitational waves around 2016, we knew all the event names by heart. Those days are gone.</p>

<h2>Part II: The Companion Papers (Brief Overview)</h2>

<ol>
  <li><strong>Intro:</strong> <a href="https://arxiv.org/abs/2605.27223">arXiv:2605.27223</a> — overview of observing runs, detector network, and catalog conventions</li>
  <li><strong>Methods:</strong> <a href="https://arxiv.org/abs/2605.27224">arXiv:2605.27224</a> — how raw data become a catalog of events</li>
  <li><strong>Open Data:</strong> <a href="https://arxiv.org/abs/2605.27090">arXiv:2605.27090</a> — what data are publicly available and how to access them</li>
  <li><strong>GWTC-5 Catalog:</strong> <a href="https://arxiv.org/abs/2605.27225">arXiv:2605.27225</a> — the new detections from O4b ⭐</li>
  <li><strong>GW Populations:</strong> <a href="https://arxiv.org/abs/2605.27226">arXiv:2605.27226</a> — population properties of compact binaries ⭐</li>
  <li><strong>Constraints on the Cosmic Expansion Rate:</strong> <a href="https://arxiv.org/abs/2605.27227">arXiv:2605.27227</a></li>
  <li><strong>Tests of General Relativity</strong> (to be published)</li>
  <li><strong>Searches for GW Lensing Signatures</strong> (to be published)</li>
</ol>

<p>The <strong>Methods paper</strong> describes the full pipeline from raw detector data to a catalog entry. The table below shows the different independent search pipelines used — each has its own strengths, and having multiple is important since some events are only found by one pipeline.</p>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot-2026-05-29-at-9.19.29-AM.png" alt="Table 3: Search pipelines used in O4b analysis">
  <div class="fig-caption"><strong>Table 3</strong> from the Methods paper: An overview of the different GW search pipelines used in the O4b analysis.</div>
</div>

<p>The <strong>Open Data paper</strong> sets a high standard for open science — every figure in the papers can be reproduced from downloadable data files, with independent parameter-estimation pipelines from groups outside LVK also publicly available. That is not trivial, and it is something our community should be proud of.</p>

<h2>Part III: The Catalog Paper — New Detections from O4b</h2>

<h3>The Numbers</h3>

<div class="highlight-box">
<ul style="margin:0; padding-left:1.3em;">
  <li><strong>161 compact binary coalescence candidates</strong> with p<sub>astro</sub> &gt; 0.5</li>
  <li><strong>104 events with FAR &lt; 1 yr<sup>−1</sup></strong> — high-confidence catalog (~88% purity)</li>
  <li><strong>All consistent with binary black holes (BBH)</strong> — no BNS or NSBH systems</li>
  <li><strong>5 BBH signals with network SNR &gt; 30</strong>, with the highest ever recorded SNR of <strong>76.9 for GW250114_082203</strong></li>
  <li>Combined with previous catalogs: <strong>390 total candidates with p<sub>astro</sub> ≥ 0.5</strong></li>
</ul>
</div>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot-2026-05-29-at-9.44.21-AM.png" alt="Mass contours for all O4b events">
  <div class="fig-caption"><strong>Figure 3</strong> (top) from the Catalog paper: 90% credible-region contours in primary vs secondary mass for all O4b candidates with FAR &lt; 1 yr<sup>−1</sup>.</div>
</div>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot-2026-05-29-at-9.42.54-AM.png" alt="Total mass vs mass ratio contours for O4b events">
  <div class="fig-caption"><strong>Figure 3</strong> (bottom): 90% credible-region contours in total mass vs mass ratio for all O4b candidates.</div>
</div>

<h3>Highlighted Events</h3>

<div class="event-card">
  <div class="event-name">GW241011_233834 — The Unequal-Mass Surprise</div>
  <p>Total mass ~25 M<sub>☉</sub>, mass ratio ~1:3, with a misaligned primary spin (χ<sub>eff</sub> ≈ +0.5) — suggesting a possible <strong>hierarchical merger</strong> origin in a dense stellar environment. The closest of the new O4b candidates, at ~0.21 Gpc.</p>
</div>

<div class="event-card">
  <div class="event-name">GW241110_124123 — A Possible Negative-Spin Candidate</div>
  <p>May be the first GW event to <em>require</em> a negative effective inspiral spin (χ<sub>eff</sub> = −0.31<sup>+0.23</sup><sub>−0.18</sub>). Another possible hierarchical merger candidate. I'll return to what this means for spin population inference below.</p>
</div>

<div class="event-card">
  <div class="event-name">GW240615_113620 — Best Localized GW Source Ever</div>
  <p>90% credible sky area of just <strong>6 deg<sup>2</sup></strong> — an extraordinary improvement enabling much more targeted electromagnetic follow-up. Typical GW events are localized to hundreds or thousands of square degrees.</p>
</div>

<div class="event-card">
  <div class="event-name">GW250114_082203 — The Loudest Event Ever</div>
  <p>The highest network SNR ever recorded: <strong>76.9</strong>. For reference, GW150914 — the first detection — had an SNR of about 24. This allows very precise measurements of source properties and stringent tests of general relativity.</p>
</div>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot-2026-05-29-at-9.47.29-AM.png" alt="Chirp mass vs chi_eff contours for highlighted O4b events">
  <div class="fig-caption"><strong>Figure 4</strong> from the Catalog paper: 90% credible-region contours in chirp mass ℳ vs effective inspiral spin χ<sub>eff</sub> for the highlighted O4b candidates.</div>
</div>

<h2>Part IV: The Populations Paper</h2>

<p>The Populations paper (<a href="https://arxiv.org/abs/2605.27226">arXiv:2605.27226</a>) asks: what is the distribution of masses, spins, and merger rates across the full population? Two complementary approaches are used:</p>

<table style="font-size:0.9em; border-collapse:collapse; margin: 1em 0; width:100%;">
  <thead>
    <tr style="background:#f0f0f0;">
      <th style="padding:0.4em 0.8em; border:1px solid #ddd;">Parametric model (FullPop)</th>
      <th style="padding:0.4em 0.8em; border:1px solid #ddd;">Non-parametric model (PixelPop)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="padding:0.4em 0.8em; border:1px solid #ddd;">Assumes a specific functional form; infers a small set of parameters. Strong assumptions, low statistical uncertainty.</td>
      <td style="padding:0.4em 0.8em; border:1px solid #ddd;">Divides parameter space into bins; infers rate in each bin directly. Fewer model assumptions, but more uncertainty.</td>
    </tr>
  </tbody>
</table>

<h3>Merger Rates</h3>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot-2026-05-29-at-9.58.09-AM.png" alt="Merger rates table">
  <div class="fig-caption"><strong>Table 2</strong> from the Populations paper: Inferred merger rates in Gpc<sup>−3</sup> yr<sup>−1</sup> for BNS, NSBH, BBH, and IMBH binaries.</div>
</div>

<ul>
  <li>The <strong>BNS rate has decreased somewhat</strong> compared to earlier estimates — earlier high estimates were heavily influenced by GW170817, a very nearby event. As the sample grows, the rate converges to something more reliable.</li>
  <li>The <strong>BBH rate remains broadly consistent</strong> with previous estimates, with slightly smaller uncertainties.</li>
  <li>There is a <strong>non-zero IMBH rate</strong> — tantalizing, but very uncertain.</li>
</ul>

<h3>Mass Distribution</h3>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot-2026-05-29-at-9.59.11-AM.png" alt="Primary mass and mass ratio distributions">
  <div class="fig-caption"><strong>Figure 2</strong> from the Populations paper: Primary mass distribution (left) and mass ratio distribution (right) for the BBH population.</div>
</div>

<ul>
  <li><strong>No empty gap between 3–5 M<sub>☉</sub>.</strong> GWTC-5 rules out a completely empty lower mass gap — this is now solidly established.</li>
  <li><strong>Features at ~10 M<sub>☉</sub> and ~35 M<sub>☉</sub></strong> persist across models. Their origin is debated.</li>
  <li><strong>No clean pair-instability supernova (PISN) gap.</strong> The distribution extends smoothly past 50 M<sub>☉</sub> — likely because hierarchical mergers in dense environments fill in any intrinsic PISN gap.</li>
  <li>The <strong>mass ratio distribution peaks near q = 1</strong> (equal mass), declining gradually toward more unequal ratios.</li>
</ul>

<h3>The χ<sub>eff</sub> Puzzle</h3>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot-2026-05-29-at-10.00.10-AM.png" alt="Chi_eff distribution from populations paper">
  <div class="fig-caption"><strong>Figure 4</strong> from the Populations paper: Population-level posterior on χ<sub>eff</sub> (left) and χ<sub>p</sub> (right). The inset shows the asymmetry parameter δχ = p(χ<sub>eff</sub> &gt; 0) − p(χ<sub>eff</sub> &lt; 0), which is clearly positive.</div>
</div>

<p>This is the result I find most striking — and most confusing:</p>
<ul>
  <li>The χ<sub>eff</sub> distribution is <strong>asymmetric</strong>: more systems have spins aligned with the orbit than anti-aligned.</li>
  <li><strong>At least 9–40% of mergers must originate from preferentially aligned channels</strong> (e.g., isolated binary evolution) to explain the asymmetry.</li>
  <li>Yet the models also find that <strong>~39% of binaries have negative χ<sub>eff</sub></strong> — which, if true, would imply the majority of events come from dynamical formation.</li>
</ul>

<p>My honest take: I am not convinced. Spin inference is notoriously difficult and strongly correlated with mass ratio. The PixelPop smoothness prior will always spread a near-zero distribution into both positive and negative territory. I want to see more high-SNR events like GW241110 that individually require negative χ<sub>eff</sub> before drawing firm conclusions. That said, the positive asymmetry is real and persistent — at least some isolated binary evolution contribution is hard to avoid.</p>

<h3>The χ<sub>eff</sub>–q Correlation: a Puzzle That Is Fading</h3>

<p>Since GWTC-2.0, several analyses had reported a trend where more unequal-mass systems tend to have higher χ<sub>eff</sub>. GWTC-5.0 finds <strong>decreased evidence that the <em>mean</em> of χ<sub>eff</sub> evolves with q</strong> — suggesting the earlier signal may have been partly a statistical fluctuation, which simplifies the formation interpretation considerably. A broadening of the χ<sub>eff</sub> distribution at certain mass ratios may still be real, and warrants follow-up.</p>

<h3>Redshift Evolution</h3>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot-2026-05-29-at-10.01.09-AM.png" alt="BBH redshift distribution">
  <div class="fig-caption"><strong>Figure 5</strong> from the Populations paper: The BBH merger rate as a function of redshift. The dashed blue line shows the star-formation rate. The inferred slope is slightly shallower than previous estimates.</div>
</div>

<p>The BBH merger rate rises with redshift, broadly following the star-formation rate — as expected. But the new inferred slope is slightly shallower than in previous catalogs. This may favor longer delay times between star formation and merger, or a steeper metallicity dependence.</p>

<h2>Final Thoughts</h2>

<p>GWTC-5 is an extraordinary release. A few things I personally find most exciting or most puzzling:</p>

<ul>
  <li><strong>No neutron star detections in O4b.</strong> Binary neutron stars are rare — or their merger rate is lower than early estimates. For those of us studying r-process enrichment and heavy element origins, this matters.</li>
  <li><strong>The ~10 M<sub>☉</sub> and ~35 M<sub>☉</sub> features are real and persistent.</strong> These are crying out for a systematic comparison to theoretical models across a large range of stellar physics assumptions.</li>
  <li><strong>No PISN gap.</strong> Multiple formation channels are clearly overlapping in the observed spectrum.</li>
  <li><strong>The χ<sub>eff</sub>–q mean correlation is weakening</strong> — good news for formation theory.</li>
  <li><strong>The spin story is genuinely confusing.</strong> Something about inferring populations from noisy individual measurements is making this hard to interpret. I'd rather wait for more high-SNR events before drawing firm formation-channel conclusions.</li>
  <li><strong>GW250114 with SNR = 76.9 is a gift.</strong> High-SNR events do more science per event than many low-SNR detections combined. Improving detector sensitivity is genuinely the best path forward.</li>
</ul>

<p>It's a great time to be in this field.</p>

<p class="caveat"><em>Note: This is a personal summary written from an astrophysics/formation-theory perspective. For the authoritative results, please refer directly to the LVK papers linked above. All figures are from the LVK GWTC-5 papers, reproduced here for educational commentary.</em></p>

  </div>
</details>
