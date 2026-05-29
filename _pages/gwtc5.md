---
layout: archive
title: "GWTC-5: My Summary of the New Gravitational Wave Catalog"
permalink: /gwtc5/
author_profile: true
---

<style>
.gwtc-body {
  font-size: 0.96em;
  line-height: 1.75;
  max-width: 820px;
}
.gwtc-body h2 {
  border-bottom: 1px solid #ddd;
  padding-bottom: 0.3em;
  margin: 2em 0 0.8em;
  font-size: 1.25em;
}
.gwtc-body h3 {
  margin: 1.5em 0 0.5em;
  font-size: 1.05em;
}
.gwtc-body p {
  margin: 0.7em 0 0.9em;
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
.papers-list {
  padding-left: 1.4em;
  margin: 0.7em 0;
}
.papers-list li {
  margin: 0.35em 0;
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

<div class="gwtc-body">

<p><em>Posted May 29, 2026 — This is my astrophysics-focused summary of the new GWTC-5 gravitational-wave catalog papers released by the LIGO–Virgo–KAGRA (LVK) collaboration. It is a biased summary: I come at this from the angle of trying to use gravitational-wave data to understand the lives of massive stars, and the results I find most exciting reflect that. I gave a talk on this for the group this week; some of the thoughts below are drawn from that discussion.</em></p>

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
  <div class="fig-caption">The growing stellar graveyard: gravitational-wave detections from O1 through O4b, visualized by mass. Orange dots are black hole–black hole mergers; the stellar graveyard has grown from ~3 events to over 390 candidates. Note how sparsely populated the neutron star regime (orange dots at the low-mass end) remains by O4b.</div>
</div>

<p>Below is the official timeline of observing runs from the Intro paper. Between runs, LVK improves their detectors — sometimes substantially — so each new run typically covers a larger sensitive volume. The increase in detection rate is not just a matter of running longer; it reflects real engineering improvements including quantum squeezing, upgraded laser power, and better noise characterization.</p>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot%202026-05-29%20at%209.07.25%20AM.png" alt="Timeline of LVK observing runs O1 through O4b">
  <div class="fig-caption"><strong>Figure 1</strong> from the Intro paper (<a href="https://arxiv.org/abs/2605.27223">arXiv:2605.27223</a>): Timeline of observing runs from 2015 through the beginning of O4c in January 2025. Each colored band shows the period a given detector was online, with the typical binary neutron star inspiral range labeled. Note that Virgo was absent for O4a but returned for O4b, significantly improving sky localization.</div>
</div>

<div class="question-box">
  <div class="q-label">A question that comes up</div>
  Why is the run now split into O4a, O4b, O4c — when earlier runs were just O1, O2, O3? The simple answer is that the runs are getting longer, and the collaboration takes periodic maintenance breaks (sometimes planned, sometimes forced by instrument issues). These breaks are used to fix things, improve sensitivity, and calibrate. During a multi-year run it makes sense to label the segments separately, especially since different detectors may be online at different times. There's also a practical data-analysis reason: understanding your noise well enough to do rigorous parameter estimation is an iterative process that often improves after a run ends.
</div>

<p>The GWOSC catalog website is a fantastic resource — for anyone wanting to explore the data yourself, you can download a simple CSV of all events (with masses, spins, distances, SNRs) and play with it in a spreadsheet or Python notebook:</p>
<p><strong>→ <a href="https://gwosc.org/eventapi/html/GWTC/">GWOSC catalog: gwosc.org/eventapi/html/GWTC/</a></strong></p>

<p>The catalog now contains <strong>391 events</strong>. When I started working in gravitational waves around 2016, we knew all the event names by heart. Those days are gone.</p>

<h2>Part II: The Companion Papers (Brief Overview)</h2>

<p>Here are the eight papers in the release (2 are still to come out):</p>
<ol class="papers-list">
  <li><strong>Intro:</strong> <a href="https://arxiv.org/abs/2605.27223">arXiv:2605.27223</a> — overview of the observing runs, detector network, and catalog conventions</li>
  <li><strong>Methods:</strong> <a href="https://arxiv.org/abs/2605.27224">arXiv:2605.27224</a> — how raw data become a catalog of events with inferred source properties</li>
  <li><strong>Open Data:</strong> <a href="https://arxiv.org/abs/2605.27090">arXiv:2605.27090</a> — what data are publicly available and how to access them</li>
  <li><strong>GWTC-5 Catalog:</strong> <a href="https://arxiv.org/abs/2605.27225">arXiv:2605.27225</a> — the new detections from O4b ⭐</li>
  <li><strong>GW Populations:</strong> <a href="https://arxiv.org/abs/2605.27226">arXiv:2605.27226</a> — population properties of compact binaries ⭐</li>
  <li><strong>GWTC-5.0: Constraints on the Cosmic Expansion Rate and Modified Gravitational-wave Propagation:</strong> <a href="https://arxiv.org/abs/2605.27227">arXiv:2605.27227</a> — constraints on cosmic expansion and modified GW propagation</li>
  <li><strong> GWTC-5.0: Tests of General Relativity (to be published soon) </strong></li>
  <li><strong>GWTC-5.0: Searches for Gravitational Wave Lensing Signatures (to be published) </strong></li>
</ol>

<p>I'm most interested in papers 4 and 5, which are what I'll focus on below. But a quick note on a few of the others:</p>

<p>The <strong>Methods paper</strong> describes the full pipeline from raw detector data to a catalog entry: how signals are found, how fake events ("glitches") are vetoed, how false-alarm rates are estimated, and how source properties like masses and spins are inferred via Bayesian parameter estimation. A key thing to appreciate is how many different independent search pipelines are involved. The table below shows some of them. Each pipeline has its own strengths and weaknesses, and having multiple is important — some events are only found by one pipeline.</p>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot%202026-05-29%20at%209.19.29%20AM.png" alt="Table 3: Search pipelines used in O4b analysis">
  <div class="fig-caption"><strong>Table 3</strong> from the Methods paper (<a href="https://arxiv.org/abs/2605.27224">arXiv:2605.27224</a>): An overview of the different GW search pipelines used in the O4b analysis. They differ in how they model waveforms, handle noise, and rank candidates.</div>
</div>

<p>The <strong>Open Data paper</strong> is a user guide to everything LVK has made publicly available — raw strain data, posterior samples for each event, and reproducible figure notebooks. I want to highlight this because I think it genuinely sets a high standard for open science. The community has put enormous effort into making the data immediately usable by anyone, including independent parameter-estimation pipelines from groups outside LVK. Every figure in the papers can be reproduced from downloadable data files. That is not trivial, and it is something our community should be proud of and replicate.</p>

<h2>Part III: The Catalog Paper — New Detections from O4b</h2>

<h3>The Numbers</h3>

<div class="highlight-box">
<ul style="margin:0; padding-left:1.3em;">
  <li><strong>161 compact binary coalescence candidates</strong> with p<sub>astro</sub> &gt; 0.5 (the astrophysical origin probability)</li>
  <li><strong>104 events with FAR &lt; 1 yr<sup>−1</sup></strong> — a false-alarm rate of less than once per year — for which LVK performed detailed parameter estimation; these form the high-confidence catalog (~88% purity)</li>
  <li><strong>All consistent with binary black holes (BBH)</strong> based on inferred masses — no binary neutron stars (BNS), no neutron star–black hole (NSBH) systems</li>
  <li><strong>5 BBH signals with network SNR &gt; 30</strong>, with the highest ever recorded SNR of <strong>76.9 for GW250114_082203</strong></li>
  <li>Combined with previous catalogs: <strong>390 total candidates with p<sub>astro</sub> ≥ 0.5</strong></li>
</ul>
</div>

<div class="question-box">
  <div class="q-label">A question that comes up</div>
  What's the difference between p<sub>astro</sub> and the false-alarm rate (FAR)? The FAR is a purely noise-based statement: how often would this pipeline produce a trigger of this significance from noise alone? The p<sub>astro</sub> also incorporates information about whether the signal looks like the rest of the astrophysical population (e.g., does it have masses consistent with a compact binary?). A p<sub>astro</sub> = 0.5 threshold is quite lenient — up to half those events could be noise. The FAR &lt; 1 yr<sup>−1</sup> threshold for parameter estimation is stricter and gives a higher-purity sample.
</div>

<p>The full catalog table is large, but here is part of it — all the O4b events, listed by date with their total mass, component masses, effective spin χ<sub>eff</sub>, luminosity distance, sky area, and SNR:</p>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot%202026-05-29%20at%209.37.33%20AM.png" alt="GWTC-5 catalog table part 1">
  <img src="/files/news/GWTC-5/Screenshot%202026-05-29%20at%209.37.56%20AM.png" alt="GWTC-5 catalog table part 2" style="margin-top:0.5em;">
  <div class="fig-caption"><strong>Table 2</strong> from the Catalog paper (<a href="https://arxiv.org/abs/2605.27225">arXiv:2605.27225</a>): O4b events with FAR &lt; 1 yr<sup>−1</sup>, including total mass M, chirp mass ℳ, component masses m<sub>1</sub> and m<sub>2</sub>, effective inspiral spin χ<sub>eff</sub>, luminosity distance D<sub>L</sub>, redshift z, sky localization area ΔΩ, and network SNR.</div>
</div>

<p>The figure below shows the 90% credible-region contours for all O4b events in the m<sub>1</sub>–m<sub>2</sub> mass plane (top) and the total mass–mass-ratio plane (bottom), with highlighted events in color:</p>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot%202026-05-29%20at%209.44.21%20AM.png" alt="Mass contours for all O4b events">
  <div class="fig-caption"><strong>Figure 3</strong> (top) from the Catalog paper: 90% credible-region contours in primary vs secondary mass for all O4b candidates with FAR &lt; 1 yr<sup>−1</sup>. Colored contours highlight specific events discussed in the text.</div>
</div>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot%202026-05-29%20at%209.42.54%20AM.png" alt="Total mass vs mass ratio contours for O4b events">
  <div class="fig-caption"><strong>Figure 3</strong> (bottom) from the Catalog paper: 90% credible-region contours in total mass vs mass ratio for all O4b candidates. The highlighted events (GW241011, GW241110, GW250114 etc.) stand out clearly.</div>
</div>

<h3>Highlighted Events</h3>

<div class="event-card">
  <div class="event-name">GW240925_005809 — The Calibration Gold Standard</div>
  <p>Network SNR of 31.9. This is a high-quality event used to inform detector calibration studies.</p>
</div>

<div class="event-card">
  <div class="event-name">GW241011_233834 — The Unequal-Mass Surprise</div>
  <p>Total mass ~25 M<sub>☉</sub>, with a primary of ~20 M<sub>☉</sub> and a secondary of ~6 M<sub>☉</sub> — a mass ratio of roughly 1:3. The primary has a well-measured spin that is <em>misaligned</em> with the orbit, with a positive effective inspiral spin χ<sub>eff</sub> ≈ +0.5. The misaligned spin and mass ratio suggest a possible <strong>hierarchical merger</strong> origin — the idea that the primary black hole is itself the product of a previous black hole merger — pointing to formation in a dense stellar environment (e.g., a globular cluster or nuclear star cluster). With a luminosity distance of just ~0.21 Gpc, this is likely the closest of the new O4b candidates.</p>
  <p>A caveat: hierarchical merger models might typically produce more massive black holes at this stage (think 25+20 rather than 20+6), with perhaps only the 1G (first-generation) black holes producing the really lower-mass end — see e.g. <a href="https://arxiv.org/pdf/2208.01081">arXiv:2208.01081</a> (Figure 1). That said, <a href="https://arxiv.org/pdf/2507.07183">arXiv:2507.07183</a> do find low-mass (&lt;15 M<sub>☉</sub>) black holes from cluster formation, though it remains unclear whether those models would produce systems matching <em>all</em> of the observed properties of GW241011_233834 simultaneously — the unequal mass ratio, the spin, and the individual masses. So the picture is intriguing but not clean, and this is one where I would love to see detailed model comparisons.</p>
</div>

<div class="event-card">
  <div class="event-name">GW241110_124123 — Another Unequal-Mass Candidate</div>
  <p>Another unequal-mass system, with a spinning primary roughly twice as massive as the secondary — also a possible hierarchical merger candidate. The mass ratio is less well-constrained here.</p>
  <p>This event is especially interesting because it may be the first gravitational-wave event to <em>require</em> a negative effective inspiral spin (χ<sub>eff</sub> &lt; 0), with a 90% credible interval of roughly −0.31 to +0.23. I'll return to this below — it is one of the most puzzling aspects of the entire GWTC-5 release.</p>
</div>

<div class="event-card">
  <div class="event-name">GW240615_113620 — Best Localized GW Source Ever</div>
  <p>The most precisely localized gravitational-wave source to date, with a 90% credible sky area of just <strong>6 deg<sup>2</sup></strong>. For context, typical GW events are localized to hundreds or even thousands of square degrees. This is an extraordinary improvement that enables much more targeted electromagnetic follow-up.</p>
</div>

<div class="event-card">
  <div class="event-name">GW250114_082203 — The Loudest Event Ever</div>
  <p>A BBH with the highest network SNR ever recorded: <strong>76.9</strong>. For reference, GW150914 — the first detection — had an SNR of about 24. This unprecedented signal quality allows for very precise measurements of source properties and stringent tests of general relativity. This is the kind of event that the whole community gets excited about.</p>
</div>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot%202026-05-29%20at%209.47.29%20AM.png" alt="Chirp mass vs chi_eff contours for highlighted O4b events">
  <div class="fig-caption"><strong>Figure 4</strong> from the Catalog paper: 90% credible-region contours in chirp mass ℳ vs effective inspiral spin χ<sub>eff</sub> for the highlighted O4b candidates. Note the green contour (GW241011) firmly above zero, the dark green contour (GW241110) straddling zero with a possible negative tail, and the purple contour (GW250114) at high chirp mass.</div>
</div>

<h3>The Spin Puzzle (Preview)</h3>

<p>One of the most intriguing aspects to note at the catalog level is the overall picture of effective inspiral spins. Out of ~300 gravitational-wave detections to date:</p>
<ul>
  <li>Roughly 4–10 events clearly <em>require</em> a positive χ<sub>eff</sub> (spin aligned with the orbit)</li>
  <li><strong>Essentially no event clearly requires a negative χ<sub>eff</sub></strong> — until possibly GW241110, which still has large uncertainties</li>
  <li>The vast majority of events are consistent with χ<sub>eff</sub> ≈ 0 (small or zero spins)</li>
</ul>

<p>This is already puzzling from a formation standpoint: if binary black holes formed purely through dynamical processes (e.g., in globular clusters), you'd expect spin orientations to be random — equally likely to be aligned or anti-aligned with the orbit, giving a symmetric χ<sub>eff</sub> distribution around zero. The fact that we see more events with <em>positive</em> χ<sub>eff</sub> already suggests some contribution from isolated binary evolution, where tidal interactions tend to align spins. But the full picture from the Populations paper (below) makes this even more puzzling.</p>

<h2>Part IV: The Populations Paper — What the Catalog Tells Us Collectively</h2>

<p>The Populations paper (<a href="https://arxiv.org/abs/2605.27226">arXiv:2605.27226</a>) takes all the gravitational-wave events — not just the new O4b ones — and infers what the underlying population of binary black holes and neutron stars looks like. Rather than characterizing individual events, it asks: what is the distribution of masses, spins, and merger rates across the population?</p>

<p>Two complementary modeling approaches are used throughout:</p>

<table style="font-size:0.9em; border-collapse:collapse; margin: 1em 0;">
  <thead>
    <tr style="background:#f0f0f0;">
      <th style="padding:0.4em 0.8em; border:1px solid #ddd;">Parametric model (FullPop)</th>
      <th style="padding:0.4em 0.8em; border:1px solid #ddd;">Non-parametric model (PixelPop)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="padding:0.4em 0.8em; border:1px solid #ddd;">Assumes a specific functional form (e.g., broken power law + Gaussian peaks); infers a small set of parameters</td>
      <td style="padding:0.4em 0.8em; border:1px solid #ddd;">Divides parameter space into bins; infers the rate in each bin directly, assuming only smoothness between adjacent bins</td>
    </tr>
    <tr>
      <td style="padding:0.4em 0.8em; border:1px solid #ddd;">Strong assumptions, low statistical uncertainty</td>
      <td style="padding:0.4em 0.8em; border:1px solid #ddd;">Fewer model assumptions, but more uncertainty; can miss sharp features due to smoothing</td>
    </tr>
  </tbody>
</table>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot%202026-05-29%20at%209.57.02%20AM.png" alt="2D mass distribution from populations paper">
  <div class="fig-caption"><strong>Figure 1</strong> from the Populations paper (<a href="https://arxiv.org/abs/2605.27226">arXiv:2605.27226</a>): Differential merger rate as a function of both component masses m<sub>1</sub> and m<sub>2</sub>, for the FullPop (left) and PixelPop (right) models. The striking flat region at low primary masses in the PixelPop result arises partly as a modeling artifact — an overly flat prior — rather than a genuine astrophysical feature.</div>
</div>

<h3>Merger Rates</h3>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot%202026-05-29%20at%209.58.09%20AM.png" alt="Merger rates table">
  <div class="fig-caption"><strong>Table 2</strong> from the Populations paper: Inferred merger rates in Gpc<sup>−3</sup> yr<sup>−1</sup> for binary neutron stars (BNS), neutron star–black hole binaries (NSBH), binary black holes (BBH), and intermediate-mass black hole binaries (IMBH).</div>
</div>

<p>A few things to note from the rates:</p>
<ul>
  <li>The <strong>BNS rate has decreased somewhat</strong> compared to earlier estimates. I'm actually not worried about this — the earlier high estimates were heavily influenced by GW170817, a very nearby and loud event. When you observe one event that close, you extrapolate to many more at larger distances, inflating your rate estimate. As the sample grows and becomes more representative, the rate naturally converges to something more reliable.</li>
  <li>The <strong>BBH rate remains broadly consistent</strong> with previous estimates, with slightly smaller uncertainties.</li>
  <li>There is a <strong>non-zero IMBH rate</strong> — tantalizing, but very uncertain.</li>
</ul>

<h3>Mass Distribution</h3>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot%202026-05-29%20at%209.59.11%20AM.png" alt="Primary mass and mass ratio distributions">
  <div class="fig-caption"><strong>Figure 2</strong> from the Populations paper: Primary mass distribution (left) and mass ratio distribution (right) for the BBH population. Blue = PixelPop (GWTC-5), red = FullPop (GWTC-5), black = FullPop (GWTC-4). Dashed vertical lines indicate the 1% boundary of the parameter estimation prior — results in hatched regions should be treated with care.</div>
</div>

<p>Key results from the mass distribution:</p>
<ul>
  <li><strong>No empty gap between 3–5 M<sub>☉</sub></strong>. With GWTC-5, the models rule out a completely empty "lower mass gap." This is now very solidly established: binary black holes do form in what was historically thought to be a forbidden mass range.</li>
  <li><strong>Features at ~10 M<sub>☉</sub> and ~35 M<sub>☉</sub></strong> in the primary mass distribution continue to appear across models. Their origin is debated — they may reflect features in the stellar initial mass function, the pair-instability supernova mass spectrum, or something else entirely.</li>
  <li>The distribution extends to high masses without going to zero, confirming that BBH systems with m<sub>1</sub> ~ 70–100 M<sub>☉</sub> do form and merge.</li>
  <li>The <strong>mass ratio distribution peaks near q = 1</strong> (equal mass), with evidence for a gradual decline toward more unequal mass ratios.</li>
</ul>

<div class="question-box">
  <div class="q-label">A question that comes up</div>
  Is the total mass in the catalog table just m<sub>1</sub> + m<sub>2</sub>? Roughly yes, but these are all inferred independently through Bayesian parameter estimation — the chirp mass and total mass are typically better constrained than the individual masses, so they're not just derived quantities. Be careful: never compute statistics by simply adding the median of m<sub>1</sub> to the median of m<sub>2</sub>. The joint posterior distribution can be highly correlated and asymmetric, and naive arithmetic on medians can introduce significant biases.
</div>

<h3>Spin Distribution</h3>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot%202026-05-29%20at%209.59.46%20AM.png" alt="Spin magnitude and tilt distributions">
  <div class="fig-caption"><strong>Figure 3</strong> from the Populations paper: Differential BBH merger rate as a function of spin magnitude (left) and tilt angle cos θ (right). There is a concentration of events near zero spin magnitude and some preference for aligned (cos θ → 1) spins, though both models show significant uncertainty.</div>
</div>

<p>The spin results are fascinating and somewhat puzzling. Most BBH systems have small spin magnitudes — the population peaks near zero. But there is a subset with meaningfully large spins, and the tilt distribution shows some preference toward alignment.</p>

<h3>The Chi_eff Puzzle</h3>

<p>This is the result I find most striking — and most confusing — from this entire release. Here is Figure 4 from the Populations paper:</p>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot%202026-05-29%20at%2010.00.10%20AM.png" alt="Chi_eff distribution from populations paper">
  <div class="fig-caption"><strong>Figure 4</strong> from the Populations paper: Population-level posterior on the effective inspiral spin χ<sub>eff</sub> (left) and precessing spin χ<sub>p</sub> (right). Blue = PixelPop, red = Bivariate Skewed χ<sub>eff</sub>/χ<sub>p</sub> model (GWTC-5), black = SkewNormal (GWTC-4). The inset shows the asymmetry parameter δχ = p(χ<sub>eff</sub> &gt; 0) − p(χ<sub>eff</sub> &lt; 0), which is clearly positive.</div>
</div>

<p>What the paper finds:</p>
<ul>
  <li>The χ<sub>eff</sub> distribution is <strong>asymmetric</strong>: more probability lies above zero than below, meaning more systems have spins preferentially aligned with the orbital angular momentum.</li>
  <li>By calculating the union of 90% credible intervals, they estimate that <strong>at least 9–40% of mergers must originate from preferentially aligned channels</strong> (e.g., isolated binary evolution) to explain the observed asymmetry.</li>
  <li>At the same time, they find that <strong>39 ± 7% of binaries have negative χ<sub>eff</sub></strong> (according to the Bivariate Skewed model; 36 ± 6% from PixelPop), indicating systems with at least one black hole spin misaligned by more than 90° with respect to the orbit.</li>
</ul>

<p>Here is where it gets confusing. If you take the 39% negative χ<sub>eff</sub> value at face value, you would reason: for every misaligned (negative χ<sub>eff</sub>) system, a purely dynamical channel should produce an equally likely aligned one. So if ~40% are negative, then ~40% should be positive from the same channel, meaning ~80% of all events come from dynamically formed systems. That is a very strong claim — and it seems to be in tension with what you see from individual events, where only a handful clearly require positive χ<sub>eff</sub> and almost none clearly require negative χ<sub>eff</sub>.</p>

<p>My honest take: I am not convinced. The χ<sub>eff</sub> measurement is notoriously difficult — it is strongly correlated with the mass ratio and other parameters, and spin inference from current detectors is genuinely hard. Furthermore, the PixelPop approach has a known limitation: even if the true χ<sub>eff</sub> distribution were a delta function at zero, the smoothness prior would spread it into both positive and negative territory. So a distribution that peaks near zero will always "leak" into the negative. I think the evidence for a significant negative-χ<sub>eff</sub> population is intriguing but not yet compelling. I want to see a few more events like GW241110 — ones that individually require negative χ<sub>eff</sub> — before drawing strong conclusions.</p>

<p>That said, the asymmetry toward positive χ<sub>eff</sub> is real and persistent across catalogs. At least some fraction of binary black holes does form through a channel that aligns spins — almost certainly including some contribution from isolated binary evolution. The question of <em>how much</em> remains very much open.</p>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot%202026-05-29%20at%2010.01.22%20AM.png" alt="10 solar mass feature mass ratio and spin distributions">
  <div class="fig-caption"><strong>Figure 6</strong> from the Populations paper: Mass ratio distribution (top) and effective spin distribution (bottom) for systems near the ~10 M<sub>☉</sub> peak (red), compared to the rest of the population (blue), inferred from three models (FullPop, PixelPop, and a Binned Gaussian Process). Systems near the 10 M<sub>☉</sub> feature tend to have mass ratios near q ~ 1 and a distinct spin distribution — a potential signature of a specific formation pathway.</div>
</div>

<h3>Isolating the 10 M<sub>☉</sub> Feature</h3>

<p>One of the neatest analyses in the Populations paper is an attempt to characterize the ~10 M<sub>☉</sub> feature in isolation. By comparing the mass ratio and spin distributions of BBH systems near the 10 M<sub>☉</sub> peak to the rest of the population, the paper finds that these systems tend to be more symmetric in mass ratio (q closer to 1) and show a different spin distribution. This is suggestive of a distinct formation pathway — possibly isolated binary evolution, where mass transfer naturally tends to produce near-equal-mass remnants. Testing this more rigorously with large grids of theoretical models is something I think is genuinely valuable, and not yet done systematically in the literature.</p>

<h3>Redshift Evolution</h3>

<div class="fig-block">
  <img src="/files/news/GWTC-5/Screenshot%202026-05-29%20at%2010.01.09%20AM.png" alt="BBH redshift distribution">
  <div class="fig-caption"><strong>Figure 5</strong> from the Populations paper: The BBH merger rate as a function of redshift (left), with the inferred redshift evolution index κ<sub>z</sub> (right). The dashed blue line shows the star-formation rate for comparison. The inferred slope is slightly lower than previous estimates, suggesting the BBH merger rate may not track the star-formation rate as steeply as some models predict.</div>
</div>

<p>The BBH merger rate rises with redshift, broadly following the star-formation rate — as expected, since most black holes ultimately come from massive stars that formed earlier in cosmic history. But the new inferred slope is slightly shallower than in previous catalogs. This is interesting for the modeling community: a gentler redshift evolution may favor longer delay times between star formation and merger, or a steeper metallicity dependence in the mass spectrum.</p>

<h2>Final Thoughts</h2>

<p>GWTC-5 is an extraordinary release. The sheer number of detections (390+ total) and the quality of the loudest events (SNR up to 76.9) represent a new era for gravitational-wave astronomy. A few things I personally find most exciting or most puzzling:</p>

<ul>
  <li><strong>No neutron star detections in O4b.</strong> This is not entirely surprising given the volume, but it is a reminder that binary neutron stars are rare — or at least their merger rate has decreased from early estimates. For those of us trying to understand r-process enrichment and the origin of heavy elements, this matters.</li>
  <li><strong>The ~10 M<sub>☉</sub> and ~35 M<sub>☉</sub> features in the mass spectrum are real and persistent.</strong> These are crying out for a systematic comparison to theoretical models across a large range of assumptions about stellar physics and binary evolution.</li>
  <li><strong>The spin story is genuinely confusing.</strong> The population-level analysis says ~40% of systems might have negative χ<sub>eff</sub>, yet individually we can barely find one. Something about how we infer the population from noisy individual measurements is making this hard to interpret. I'd rather wait for more high-SNR events with clear individual spin measurements before drawing firm formation-channel conclusions.</li>
  <li><strong>GW250114 with SNR = 76.9 is a gift.</strong> High-SNR events do more for science per event than many low-SNR detections combined. Improving detector sensitivity is genuinely the best way to advance the field, not just accumulating more marginal candidates.</li>
</ul>

<p>The next step is O4c, whose public alerts are already visible online. Word on the street suggests no binary neutron star events there either — though the story can always change once the full catalog analysis is done. And then O5 looms on the horizon, promising another major leap in sensitivity.</p>

<p>It's a great time to be in this field.</p>

<p class="caveat"><em>Note: This is a personal summary written from an astrophysics/formation-theory perspective. I have not read all the papers in full detail and some statements here may be imprecise. For the authoritative results, please refer directly to the LVK papers linked above. All figures are from the LVK GWTC-5 papers and are reproduced here for educational commentary.</em></p>

</div>
