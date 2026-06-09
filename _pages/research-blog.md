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

<details id="parkosidis2026eccentric">
  <summary onclick="var d=this.closest('details');setTimeout(function(){if(d.open)history.replaceState(null,'','#'+d.id);else history.replaceState(null,'',location.pathname);},0)">Parkosidis et al. 2026 — Eccentricity as a probe of mass-transfer physics: Eccentric mass transfer as a solution to the wide eccentric binary problem <span class="item-date">Jun 9, 2026</span></summary>
  <div class="details-content">

<p><em>Parkosidis, Toonen, Laplace &amp; Schaffenroth (2026) · <a href="https://arxiv.org/abs/2606.09464" target="_blank">arXiv:2606.09464</a></em></p>

<p>Cool paper on how <strong>eccentric mass transfer</strong> can shape the orbital parameters of post-mass-transfer binaries. Most binary population synthesis codes assume that mass transfer circularizes the orbit — but as I discussed in the <a href="#vanSon2026">van Son et al. 2026 entry</a>, observations of post-mass-transfer systems increasingly show that significant eccentricities are common and cannot simply be swept under the rug. This paper takes a concrete step toward modeling this properly.</p>

<p>The authors introduce the <strong>GeMT (General Mass Transfer) model</strong>, which incorporates eccentric mass transfer, and test it against a well-chosen observational benchmark: <strong>hot subdwarf B (sdB) stars paired with main-sequence companions in wide orbits</strong>. These sdB+MS binaries are particularly valuable because their orbital properties — periods, mass ratios, and eccentricities — place tight constraints on what must have happened during the mass transfer episode that formed the sdB. If a model cannot reproduce this population, something is wrong with its mass transfer physics.</p>

<p>The result is striking: the GeMT model naturally reproduces all the observed orbital parameters of wide sdB+MS binaries <em>without fine-tuning</em>. Previous models that assumed circular mass transfer struggled with this population; allowing eccentricity to develop during mass transfer resolves the tension cleanly.</p>

<p>The paper also explores <strong>different formation pathways</strong> depending on when Roche lobe overflow (RLOF) is initiated during the donor star's evolution, finding that this leads to distinct tracks in orbital-parameter space. Importantly, the eccentricity that emerges after mass transfer depends sensitively on:</p>
<ul>
  <li>The <strong>amount of mass transferred</strong></li>
  <li>The <strong>accretion efficiency</strong> (how much of the transferred mass the companion actually accretes)</li>
  <li>The <strong>angular momentum loss</strong> from the system</li>
</ul>

<p>This is the key result from a GW paleontology perspective: because the post-mass-transfer eccentricity depends on these parameters, and because we can <em>measure</em> eccentricities in observed post-mass-transfer binaries, <strong>these observations can be used to directly constrain the uncertain mass transfer physics</strong>. This is exactly the kind of observational anchor the field needs — it turns eccentricity from a nuisance into a diagnostic.</p>

<p>More broadly, this paper reinforces the message that <strong>eccentricity after mass transfer is a real and important feature that most binary evolution codes currently neglect</strong>. For GW source modeling, this matters: if the orbital parameters of binaries entering later evolutionary stages (second mass transfer, common envelope, supernova) are systematically wrong because we assumed circularization that didn't happen, our predictions for merger rates and distributions will carry a corresponding systematic error. How large that error is remains to be quantified, but papers like this one are laying the groundwork for getting it right.</p>

  </div>
</details>

<details id="boco2026bbhrate">
  <summary onclick="var d=this.closest('details');setTimeout(function(){if(d.open)history.replaceState(null,'','#'+d.id);else history.replaceState(null,'',location.pathname);},0)">Boco et al. 2026 — Can current models predict the local black hole merger rate? <span class="item-date">Jun 3, 2026</span></summary>
  <div class="details-content">

<p><em>Boco, Bosi, Sgalletta, Romagnolo &amp; Mapelli (2026) · <a href="https://arxiv.org/abs/2606.02725" target="_blank">arXiv:2606.02725</a></em></p>

<p>An interesting paper. The starting point is a familiar tension in the field: binary population synthesis models of isolated binary evolution tend to predict BBH merger rates that are on the high side compared to what LIGO–Virgo–KAGRA actually measures (~14–26 Gpc⁻³ yr⁻¹). This paper focuses on one recent simulation — and notes that several others share the same problem — where the predicted local BBH merger rate exceeds the LVK-inferred value by roughly an order of magnitude.</p>

<p>A common response to this tension has been to suggest it can "easily" be fixed by adjusting assumptions about the <strong>cosmic star formation history (SFH)</strong> — that is, how many stars form as a function of redshift, and with what metallicities. Since BBH merger rates are strongly boosted at low metallicities (lower metallicity → less mass loss → heavier black holes → higher merger rates), tweaking the metallicity evolution of the SFH can in principle move the predicted rate up or down substantially. So: can we just tune the SFH to match observations?</p>

<p>What this paper does well is take that question seriously and test it rigorously. They explore a range of different SFH assumptions and — critically — they also check whether those assumptions are consistent with <em>independent observations of the star formation history itself</em>. This is an important step that is often skipped: it is easy to pick an SFH that makes your simulation match the GW rate, but harder to do so while also remaining consistent with what we know from galaxy surveys, cosmic metallicity evolution measurements, and related observations.</p>

<p>Their finding is sobering: most SFH choices that bring the predicted BBH rate down enough to match LVK would require an unrealistically metal-rich early universe — very high metal enrichment very early, leaving almost no room for low-metallicity star formation. Since it is precisely that low-metallicity population that drives such a large fraction of the BBH rate in these simulations, suppressing it enough to fix the rate tension pushes the SFH into regimes that are observationally excluded. In other words, the SFH knob is not as free as sometimes assumed. The conclusion the authors draw is that resolving the discrepancy likely requires revisions to the stellar and binary evolution physics itself — not just the input SFH.</p>

<p>I find the paper's framing — simultaneously varying the SFH <em>and</em> comparing against SFH observations — genuinely valuable, and I think more papers should do this. It puts a much more meaningful constraint on what kinds of "fixes" are actually physically acceptable.</p>

<div class="highlight-box">
<strong>Where I personally disagree:</strong> The title asks "Can current models predict the local black hole merger rate?" and some of the conclusions suggest that no realistic isolated-binary-evolution model can produce a BBH rate as low as ~10 Gpc⁻³ yr⁻¹. I don't think this is fully correct. The simulations tested in this paper are among the higher-rate models in the literature, and in recent years there have been many simulations — and subsets of parameter-space models — that do predict rates comfortably consistent with the low end of the LVK range, at least for some combinations of physical assumptions. The conclusion that no realistic isolated binary model can produce low rates seems too strong given that landscape. The tension is real and worth taking seriously, but framing it as a fundamental breakdown of the isolated channel as a whole overstates what the current evidence actually shows.
</div>

<p>That said, this paper has made me want to think more carefully about which recent models actually do predict low BBH rates, and what the physical ingredients are that make that possible. So: <strong>more coming soon</strong> on that front — stay tuned!</p>

  </div>
</details>

<details id="broekgaarden2026ce">
  <summary onclick="var d=this.closest('details');setTimeout(function(){if(d.open)history.replaceState(null,'','#'+d.id);else history.replaceState(null,'',location.pathname);},0)">Broekgaarden et al. 2026 — How Common Are Common Envelopes? Quantifying Their Role in Forming Gravitational-Wave Sources <span class="item-date">Jun 4, 2026</span></summary>
  <div class="details-content">

  <p>Excited that my paper is out! This was a team effort: <strong>Floor S. Broekgaarden</strong>, Ana Lam, Sasha Levina, Jakub Klencki, Kyle A. Rocha, Lieke van Son, Steffani M. Grondin, Monica Gallegos-Garcia, Brian D. Metzger, Enrico Ramirez-Ruiz, Angela Twum, Melanie Santiago, Julia Haynes, Tyler B. Smith, Amedeo Romagnolo, Edo Berger, and Lucas M. de Sá<br>
  <a href="https://arxiv.org/abs/2606.05322" target="_blank">arXiv:2606.05322</a></p>

  <p>All data and results are publicly available with interactive figures and tables you can explore yourself: <a href="https://floorbroekgaarden.github.io/Rates_of_Formation_Channels/interactive_figures_and_tables/formation_channel_rates_table.html" target="_blank"><strong>[interactive catalog]</strong></a></p>

  <p>One of the most consequential — and most uncertain — phases in the life of a binary star system is <strong>common-envelope (CE) evolution</strong>. When one star grows large and engulfs its companion, the two stars spiral together inside a shared gas envelope. If the system survives, the orbit shrinks dramatically, setting up the binary to eventually merge as a pair of compact objects detectable by LIGO, Virgo, and KAGRA. If it doesn't survive, the binary is destroyed. CE evolution is therefore a critical bottleneck in forming gravitational-wave sources — yet after decades of study, we still don't fully understand it.</p>

  <p>This paper asks a deceptively simple question: <em>is CE evolution actually required to form the binary black holes, neutron stars, and black hole–neutron star systems that gravitational-wave observatories detect?</em> Rather than picking a single simulation and reporting its answer, we compiled and compared predictions from <strong>over 200 population-synthesis simulations</strong> spanning many different codes and physical assumptions, and asked what fraction of merging systems in each simulation formed through a CE phase.</p>

  <figure>
    <img src="/images/gwp-news/26_06_05/Figure2.png" alt="Figure 2: Global overview of CE fraction diversity across 200+ population-synthesis simulations for BBH, BHNS, and BNS" style="width: 100%; max-width: 860px; border-radius: 4px;">
    <figcaption><strong>Figure 2.</strong> Global overview of Level 1 formation-channel diversity across 200+ compiled population-synthesis simulations. Each point shows the fraction of systems forming with CE (x-axis) vs. without CE (y-axis) for binary black holes (BBH, 117 simulations), BH–neutron star systems (BHNS, 71 simulations), and binary neutron stars (BNS, 53 simulations). BBH and BHNS populations scatter across nearly the full allowed range — from CE-dominated to entirely CE-free — while BNS mergers cluster strongly toward the CE side. See the <a href="https://floorbroekgaarden.github.io/Rates_of_Formation_Channels/interactive_figures_and_tables/formation_channel_rates_table.html" target="_blank">interactive catalog</a> to explore individual simulations.</figcaption>
  </figure>

  <p>The headline result (Figure 2) is striking: <strong>for binary black holes and BH–neutron star systems, the simulations span nearly the full allowed range</strong> — from models where essentially every merger formed through a CE phase to models where none did — yet these same models all produce similar merger rates consistent with current LVK observations. This reveals a <strong>fundamental degeneracy</strong>: merger rates alone cannot tell us how these systems formed. We can match the data with completely opposite physical assumptions about CE evolution.</p>

  <p>Binary neutron stars tell a very different story. Across essentially all models, BNS mergers form almost exclusively through channels involving at least one CE phase (≳90–100%). This makes BNS systems a much more powerful probe of CE physics — if we can measure their merger rates and mass distributions precisely enough, we can potentially break the degeneracy that plagues the BBH population.</p>

  <figure>
    <img src="/images/gwp-news/26_06_05/Figure3.png" alt="Figure 3: Fractional CE contributions per simulation for the BBH population" style="width: 100%; max-width: 860px; border-radius: 4px;">
    <figcaption><strong>Figure 3.</strong> Fractional contributions of formation channels (with CE in blue/orange, without CE in orange, other channels in lighter colors) for every BBH simulation in the compiled catalog, sorted by CE fraction. The right panel shows the corresponding intrinsic BBH merger rate R₀ for each simulation. The enormous spread in CE fractions — from 0% to ~100% — is immediately visible, and critically, this spread is not correlated with the merger rate: simulations at both extremes of CE fraction produce rates consistent with LVK observations.</figcaption>
  </figure>

  <figure>
    <img src="/images/gwp-news/26_06_05/Figure9.png" alt="Figure 9: BBH CE fraction vs merger rate across simulation frameworks" style="width: 100%; max-width: 860px; border-radius: 4px;">
    <figcaption><strong>Figure 9.</strong> Top panel: fraction of BBH mergers forming without a CE phase vs. total intrinsic BBH merger rate, for every simulation in the catalog colored by simulation framework. Within any single framework, varying parameters can shift both the CE fraction and the merger rate, but across the full compilation there is no universal correlation: CE-free and CE-dominated models alike span the full range of observed-compatible merger rates. The bottom panels show pairwise comparisons of key model parameters, illustrating the highly non-linear and framework-dependent nature of the relationships.</figcaption>
  </figure>

  <p>The bottom line is that we need to go beyond merger-rate measurements alone. Multi-messenger observations, mass and spin distributions, delay-time distributions, and eventually electromagnetic counterparts will all be needed to break the degeneracy and constrain what CE evolution actually looks like. The interactive catalog accompanying this paper is designed to make it easy to explore the full simulation landscape and identify which observables are most diagnostic. There is much more work to do here — but this paper is intended as a community resource to anchor those future efforts.</p>

  </div>
</details>

<details id="vanSon2026">
  <summary onclick="var d=this.closest('details');setTimeout(function(){if(d.open)history.replaceState(null,'','#'+d.id);else history.replaceState(null,'',location.pathname);},0)">van Son et al. 2026 — Post-Mass-Transfer Binaries: A Living Catalog &amp; Unified Review <span class="item-date">Jun 1, 2026</span></summary>
  <div class="details-content">

<p><em>van Son, Yamaguchi, Nagarajan, Shenar, Sen, Laroche, Leiner, Sana &amp; Pols (2026) · <a href="https://arxiv.org/abs/2605.31290" target="_blank">arXiv:2605.31290</a> · <a href="https://binary-observations.github.io/post_mt_catalog/" target="_blank">Interactive Catalog</a></em></p>

<p style="font-size:0.88em; color:#666; margin-top:-0.3em;"><em>Parts of the summary below are based on text and highlights provided by lead author Lieke van Son — with thanks and credit to her and the full author team.</em></p>

<div class="highlight-box">
<strong>TLDR (credit: authors):</strong> A comprehensive living catalog of over 5,400 binary systems that have undergone mass transfer, unifying observations across multiple research communities. Non-zero eccentricities are common at all periods and system classes, with both median values and scatter increasing with period. Gaia BH and NS systems are extreme in mass ratio but otherwise consistent with the general post-mass-transfer population.
</div>

<p>Super cool paper on the arXiv today that is directly relevant for gravitational-wave paleontology — and honestly, one I've been hoping someone would write for a while.</p>

<p>Mass transfer is one of the most uncertain and consequential phases in binary stellar evolution. Whether a binary survives a mass transfer episode, and what happens to its orbital properties — separation, eccentricity, mass ratio — in the process, largely determines whether it can eventually form a merging compact object binary. Despite its central importance, mass transfer has been notoriously hard to constrain observationally, especially for massive star binaries where data has historically been very sparse. (For a great recent review of how little we know, see <a href="https://arxiv.org/pdf/2311.01865" target="_blank">Marchant &amp; Bodensteiner 2023</a>.)</p>

<p>What makes this new paper so exciting is that the observational landscape is changing — fast. New surveys like Gaia, combined with a wealth of X-ray binaries, spectroscopic binaries, pulsar binaries, and a rapidly growing body of observations of binaries with white dwarfs, are flooding us with new data. Van Son et al. bring all of these together into a single unified catalog and review — a living, community-maintained resource of over 5,400 post-mass-transfer systems — and by doing so they are able to highlight patterns that would be invisible when looking at any one population in isolation.</p>

<div class="fig-block">
  <img src="/images/research_blog/June-vanSon26/Figure1.png" alt="Overview of post-mass-transfer binary populations (van Son et al. 2026, Figure 1)">
  <div class="fig-caption"><strong>Figure 1</strong> from van Son et al. (2026): An overview of the diverse populations of binary systems included in the catalog, spanning X-ray binaries, Gaia black hole and neutron star systems, spectroscopic binaries, pulsar binaries, and wide WD+MS systems. The breadth of this compilation is itself remarkable.</div>
</div>

<p>The headline result — and the one I find most important for GW paleontology — is about <strong>eccentricity</strong>. One of the standard assumptions baked into most binary population synthesis codes (including the ones we use to model gravitational-wave sources) is that binaries circularize after mass transfer. This paper challenges that assumption head-on.</p>

<div class="fig-block">
  <img src="/images/research_blog/June-vanSon26/Figure2.png" alt="Eccentricity across post-mass-transfer populations (van Son et al. 2026, Figure 2)">
  <div class="fig-caption"><strong>Figure 2</strong> from van Son et al. (2026): Eccentricity as a function of orbital period across the full post-mass-transfer population. Non-zero eccentricities are common throughout — at all periods and across all system classes — with both the median eccentricity and its scatter increasing with period.</div>
</div>

<p>Looking at the full population together (Figure 2), a clear picture emerges: <strong>non-zero eccentricities are common throughout</strong>, across all periods and system classes. This is not a quirk of one exotic subpopulation — it appears to be a generic feature of binaries after mass transfer. The three key results I'd highlight:</p>

<ol>
  <li><strong>Post-mass-transfer systems are not circular.</strong> The data firmly constrains the median eccentricity as a function of log period, and circular is not a good description — at least for a significant subset of systems at most periods.</li>
  <li><strong>Systems from presumed high-mass donors are more eccentric than those from low-mass donors.</strong> This asymmetry is a tantalizing hint that natal kicks — the velocity kick a neutron star or black hole receives at birth — may be playing a role in pumping up eccentricities in the more massive systems.</li>
  <li><strong>The Gaia BH and NS systems are not outliers</strong> — except in mass ratio for the Gaia BHs. In terms of orbital properties, they appear to be part of the same broader post-mass-transfer population. This is a really striking result: rather than being mysterious one-off systems, these Gaia discoveries may be telling us something about binary mass transfer that applies much more generally — especially the wide WD+MS systems that have long been an outlier in our theoretical models.</li>
</ol>

<p>The interactive online version of the catalog is genuinely fantastic, and potentially even more impactful than the paper itself:</p>
<p>→ <a href="https://binary-observations.github.io/post_mt_catalog/" target="_blank"><strong>binary-observations.github.io/post_mt_catalog/</strong></a></p>
<p>You can sort, filter, and download the data; browse through interactive plots; and even <em>suggest a missing system</em> via a built-in interface to help improve the resource. This is community science done right.</p>

<p>From a GW paleontology perspective, the key takeaway is clear: <strong>we need to revisit the circularization assumption in our population synthesis simulations.</strong> If post-mass-transfer binaries are generically eccentric, then modeling their subsequent evolution — including how eccentricity affects later mass transfer episodes, supernova dynamics, and final merger timescales — matters. Eccentric mass transfer is technically hard to implement, but this paper makes the observational case for why it cannot keep being ignored. This is exactly the kind of observational anchor that GROWL-style frameworks need to pull against.</p>

<p>Big congratulations to Lieke van Son and the whole team on this one — it's a team effort and a major community resource.</p>

  </div>
</details>

<details id="gwtc5">
  <summary onclick="var d=this.closest('details');setTimeout(function(){if(d.open)history.replaceState(null,'','#'+d.id);else history.replaceState(null,'',location.pathname);},0)">GWTC-5: My Summary of the New Gravitational-Wave Catalog <span class="item-date">May 29, 2026</span></summary>
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

<details id="massquerade2026">
  <summary onclick="var d=this.closest('details');setTimeout(function(){if(d.open)history.replaceState(null,'','#'+d.id);else history.replaceState(null,'',location.pathname);},0)">Smith et al. 2026 — Massquerade: Impacts of Mass Ratio Reversals on Binary Black Hole Merger Rates and Mass Distributions <span class="item-date">May 20, 2026</span></summary>
  <div class="details-content">

  <p>Tyler B. Smith, Floor Broekgaarden, Sasha Levina, Amedeo Romagnolo, Manasvini Komandur, Melanie Santiago, Kyle A. Rocha<br>
  <a href="https://arxiv.org/abs/2605.21580" target="_blank">arXiv:2605.21580</a></p>

  <p>When two massive stars are born together in a binary system, the heavier star is expected to also produce the heavier black hole when it dies. But binary evolution can flip this expectation. Through a process called <strong>mass ratio reversal (MRR)</strong>, the initially <em>less</em> massive star can end up forming the <em>more</em> massive black hole. This happens when mass is transferred between the stars during their lives — the lighter star receives material from its companion, grows a more massive core, and ultimately collapses into a heavier black hole than the one formed by the originally dominant star. The initially less massive star is then "massquerading" as the primary.</p>

  <p>This paper investigates how common MRR is, and — crucially — how it shapes the black hole merger rate and mass distributions that gravitational-wave observatories like LIGO, Virgo, and KAGRA actually measure. The team uses two independent binary population synthesis codes, <strong>COMPAS</strong> and <strong>SEVN</strong>, to simulate large populations of binary stars from birth through to black hole merger, and compares the resulting distributions against current LVK observations.</p>

  <p>A key finding is that the two codes make qualitatively different predictions. In <strong>COMPAS</strong>, MRR systems dominate the high-mass end of the distribution (primary masses above ~20 M☉, secondary masses above ~12 M☉), while in <strong>SEVN</strong> the MRR contribution is more diffuse and remains subdominant across the full mass range. Despite this difference, both codes agree that MRR systems preferentially populate the <em>high mass-ratio regime</em> (q ≳ 0.6, meaning the two black holes have similar masses). The upshot is that the observed mass distribution cannot simply be read as a direct map of the original stellar masses — MRR blurs that connection.</p>

  <p>The paper also identifies three distinct evolutionary channels that produce MRR (Figure 6 below): (1) <strong>core growth</strong>, where stable mass transfer fattens the secondary's helium core until it collapses into the heavier black hole; (2) <strong>PPISN shrinkage</strong>, where the primary loses mass through violent pulsational pair-instability episodes and ends up lighter than the secondary; and (3) <strong>asymmetric core-collapse supernovae</strong>, where differential stripping leaves the secondary with a heavier remnant.</p>

  <figure>
    <img src="/images/massquerade_fig2.png" alt="Figure 2: BBH merger rate density broken down by MRR and non-MRR contributions for COMPAS and SEVN" style="width: 100%; max-width: 860px; border-radius: 4px;">
    <figcaption><strong>Figure 2.</strong> Intrinsic binary black hole merger rate density as a function of primary mass M₁ (top), secondary mass M₂ (middle), and mass ratio q (bottom) at redshift z ≈ 0.2, for COMPAS (left) and SEVN (right). The total population (black) is split into MRR (purple) and non-MRR (green) contributions and compared to LVK observational constraints (gray shaded regions). COMPAS predicts MRR systems dominate at high masses, while SEVN shows a more diffuse, subdominant contribution. Both models agree that MRR preferentially populates the high mass-ratio regime (q ≳ 0.6).</figcaption>
  </figure>

  <figure>
    <img src="/images/massquerade_fig6.png" alt="Figure 6: Representative evolutionary pathways leading to MRR" style="width: 100%; max-width: 860px; border-radius: 4px;">
    <figcaption><strong>Figure 6.</strong> Representative evolutionary histories for each of the three MRR channels. Each panel shows the total stellar masses (black and red) and core masses (magenta and green) of both stars as a function of time, with vertical dotted lines marking the two supernova events. From left to right: the core-growth channel in COMPAS, the core-growth channel in SEVN (illustrating how the two codes treat this process differently), the PPISN-shrinkage channel, and the asymmetric core-collapse supernova channel.</figcaption>
  </figure>

  </div>
</details>

<details id="schiebelbein2026delay">
  <summary onclick="var d=this.closest('details');setTimeout(function(){if(d.open)history.replaceState(null,'','#'+d.id);else history.replaceState(null,'',location.pathname);},0)">Schiebelbein-Zwack &amp; Fishbach 2026 — Forbidden Formation Histories: The Binary Black Hole Merger Rate Disfavors Long Delay Times <span class="item-date">May 13, 2026</span></summary>
  <div class="details-content">

<p><em>Schiebelbein-Zwack &amp; Fishbach (2026) · <a href="https://arxiv.org/abs/2605.12858" target="_blank">arXiv:2605.12858</a></em></p>

<p>Very cool paper. The central idea is an elegant inversion: the BBH merger rate is normally thought of as a convolution of the BBH <em>formation</em> rate with a delay time distribution p(t) — that is, how long it takes from when two massive stars are born to when the resulting black holes finally merge. Usually we assume a formation rate (tied to the star formation history) and a delay time distribution, and predict the resulting merger rate. Here, the authors turn this around: they take the observed BBH merger rate from GWTC-4 as input and ask what BBH formation histories and delay time distributions are consistent with it. Really cool idea.</p>

<p>In particular, they use this framework to ask which delay time distributions produce "physical" results — meaning the implied BBH formation rate must be non-negative and broadly consistent with what we'd expect from stars forming across cosmic time. The punchline is that delay time distributions with shallow power-law slopes (α ≳ −0.7) get into trouble: they concentrate too many mergers at low redshift, producing a pile-up near z ~ 0 that is hard to reconcile with the observed redshift distribution. Since shallow delay time distributions are thought to be associated with the <strong>stable mass transfer channel</strong>, the paper argues these are disfavored.</p>

<p>I find the general approach genuinely interesting — it is a direct attempt to connect the population-level GW observations back to the massive stellar binaries that formed them, without having to commit to a specific simulation. That kind of inversion is powerful in principle and I would love to see it developed further.</p>

<div class="highlight-box">
<strong>Caveats worth keeping in mind (IMHO):</strong> The results come with some significant assumptions that make it a bit difficult to tell how robust they would be in the more complex universe we probably live in:
<ol style="margin: 0.6em 0 0; padding-left: 1.4em;">
  <li><strong>Redshift-independent delay time distribution.</strong> The paper assumes p(t) does not evolve with redshift, but this is very unlikely to be true. At higher redshifts, BBHs form preferentially from lower-metallicity stars, and we have good reason to think this shapes the delay time distribution — both through its effect on the mass-transfer physics and on the black hole masses produced. The observed data likely already contain this metallicity-driven evolution baked in, so assuming a fixed p(t) may be absorbing real physical evolution into the inferred constraints.</li>
  <li><strong>Single-channel assumption.</strong> The analysis implicitly treats the BBH population as coming from one channel with one characteristic delay time distribution. But dynamical formation in dense stellar environments (globular clusters, nuclear star clusters) contributes to the observed rate and likely brings its own different delay time distribution — or more precisely, a different relationship between formation time and merger time altogether. If the dynamical channel contributes meaningfully at certain redshifts, it could mimic or mask the signatures the paper is attributing to the isolated stable mass transfer channel.</li>
  <li><strong>Shape of the delay time distribution.</strong> The conclusions depend on the assumed functional form for p(t). It is a bit unclear from the paper how exactly the delay time distribution is derived or how sensitive the results are to that choice — a more complex or bimodal shape could change the picture.</li>
</ol>
</div>

<p>All in all, an interesting paper that pushes in exactly the right direction: using the redshift evolution of the BBH merger rate as a probe of the massive star progenitors. I am definitely interested in seeing more work like this, with the caveats above incorporated!</p>

  </div>
</details>

<details id="levina2026sfh">
  <summary onclick="var d=this.closest('details');setTimeout(function(){if(d.open)history.replaceState(null,'','#'+d.id);else history.replaceState(null,'',location.pathname);},0)">Levina et al. 2026 — From cosmological simulations to binary black hole mergers: The impact of using analytical star formation history models on gravitational-wave source populations <span class="item-date">January 28, 2026</span></summary>
  <div class="details-content">

  <p>Sasha Levina, Floor Broekgaarden, Lieke van Son, Emanuele Berti, Amedeo Romagnolo, Ruediger Pakmor, Ana Lam<br>
  <a href="https://arxiv.org/abs/2601.20202" target="_blank">arXiv:2601.20202</a></p>

  <p>To predict how many binary black hole mergers gravitational-wave detectors like LIGO and Virgo should see, theorists must combine a model of how stars form across cosmic time — the <strong>star formation history (SFH)</strong> — with a model of how binary stars evolve into merging black holes. In practice, most studies use simple analytical SFH models (e.g., power laws or fits to galaxy survey data), but these are approximations of a far more complex underlying reality. This paper asks: <em>how much does the choice of analytical SFH model actually matter?</em></p>

  <p>The team uses the <strong>IllustrisTNG cosmological simulation</strong> as a ground truth for the star formation history and metallicity evolution of the universe, and compares it against four widely-used analytical SFH prescriptions. By running binary population synthesis models with <strong>COMPAS</strong> on top of each SFH, they quantify how the choice of SFH propagates through to predictions for BBH merger rates and mass distributions detectable by current and future gravitational-wave observatories.</p>

  <p>A key finding (Figure 4 below) is that the predicted merger rate can vary by up to a factor of ~2–3 depending on which analytical SFH model is used, with the differences being most pronounced at high redshifts. This has direct implications for next-generation detectors like the Einstein Telescope and Cosmic Explorer, which will be sensitive to mergers across cosmic history. The metallicity evolution built into each SFH model is the primary driver of the spread: models that assign lower metallicities to star-forming gas at high redshift predict more BBH mergers because low-metallicity stars retain more mass and more readily form heavy black holes.</p>

  <p>Figure 6 shows how the mass distributions of detectable BBH mergers shift depending on the SFH choice, with the IllustrisTNG-based prediction bracketed by the analytical models. The results underscore that SFH uncertainty is a non-negligible systematic in population-level gravitational-wave analyses — and that using cosmological simulations as a calibration anchor can help identify and bound this uncertainty.</p>

  <figure>
    <img src="/images/levina2026_fig4.png" alt="Figure 4: BBH merger rate as a function of redshift for different SFH models" style="width: 100%; max-width: 860px; border-radius: 4px;">
    <figcaption><strong>Figure 4.</strong> Binary black hole merger rate density as a function of redshift for five star formation history models: IllustrisTNG (used as ground truth), and four analytical prescriptions. The choice of SFH leads to rate differences of up to a factor of ~2–3, with the spread growing at higher redshifts where metallicity evolution assumptions diverge most strongly.</figcaption>
  </figure>

  <figure>
    <img src="/images/levina2026_fig6.png" alt="Figure 6: Detectable BBH mass distributions for different SFH models" style="width: 100%; max-width: 860px; border-radius: 4px;">
    <figcaption><strong>Figure 6.</strong> Distributions of primary mass M₁ for detectable binary black hole mergers under each SFH model, for current LIGO-Virgo sensitivity (left) and next-generation detector sensitivity (right). The IllustrisTNG prediction (black) is bracketed by the analytical models, illustrating how SFH choice shifts the relative contribution of high-mass mergers — an effect that will become increasingly important as detector sensitivity improves.</figcaption>
  </figure>

  </div>
</details>

<script>
// Open and scroll to the entry matching the URL hash on page load
(function () {
  function openHash() {
    var hash = window.location.hash.slice(1);
    if (!hash) return;
    var el = document.getElementById(hash);
    if (el && el.tagName === 'DETAILS') {
      el.open = true;
      setTimeout(function () { el.scrollIntoView({ behavior: 'smooth', block: 'start' }); }, 100);
    }
  }
  if (document.readyState === 'loading') {
    document.addEventListener('DOMContentLoaded', openHash);
  } else {
    openHash();
  }
})();
</script>
