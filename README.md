<div align="center">

<img src="https://avatars.githubusercontent.com/u/283118079?v=4" width="110" alt="Groundlens" />

# Groundlens

### Geometric methods for trustworthy models

<p>
Embedding geometry to verify <em>what an LLM says</em> · energy geometry to model <em>how a physical system behaves</em><br>
Deterministic · auditable · calibrated · explicit about its limits
</p>

[![Website](https://img.shields.io/badge/groundlens.dev-fc7604?style=for-the-badge&logo=astro&logoColor=white)](https://groundlens.dev)
[![arXiv](https://img.shields.io/badge/arXiv-Research-b31b1b?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org/search/cs?searchtype=author&query=Mar%C3%ADn,+J)
[![License: MIT](https://img.shields.io/badge/License-MIT-000000?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![LinkedIn](https://img.shields.io/badge/Javier_Marin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/javiermarinvalenzuela/)

<br>

**[Research](#-research) · [Projects](#-projects) · [Selected results](#-selected-results) · [Featured](#-featured) · [About](#-about)**

</div>

---

Groundlens is an open-source practice for **trustworthy modeling** — making the outputs of both AI systems and physical systems verifiable, with methods rooted in geometry and grounded in peer-reviewed research. Two product lines, one principle: *verification over capability — deterministic where possible, calibrated where not, and clear about where the method stops working.*

<br>

## Research

The methods are not heuristics — they come from published work.

| Paper | Idea | Link |
|---|---|---|
| **Semantic Grounding Index (SGI)** | Ratio-based grounding verification for RAG — measures whether a response engages its source via angular geometry on the unit hypersphere. | [![arXiv](https://img.shields.io/badge/arXiv-2512.13771-b31b1b)](https://arxiv.org/abs/2512.13771) |
| **A Geometric Taxonomy of Hallucinations** | Three-type hallucination classification via directional grounding (von Mises–Fisher on displacement vectors); domain calibration reaches AUROC 0.76–0.99. | [![arXiv](https://img.shields.io/badge/arXiv-2602.13224-b31b1b)](https://arxiv.org/abs/2602.13224) |
| **Rotational Dynamics of Factual Constraint Processing** | Transformers reject wrong answers by *rotating* the representation, not rescaling — with a phase transition at ~1.6B parameters. | [![arXiv](https://img.shields.io/badge/arXiv-2603.13259-b31b1b)](https://arxiv.org/abs/2603.13259) |

<sub>Plus peer-reviewed work at IEEE and ACL/SiCon venues. Full list on [arXiv](https://arxiv.org/a/marin_j_1) and [LinkedIn](https://www.linkedin.com/in/javiermarinvalenzuela/).</sub>

<br>

##  Projects

<table>
<tr>
<td width="50%" valign="top">

### Groundlens

**LLM output verification.** Geometric grounding / hallucination triage for production LLMs in regulated industries — deterministic scores, sub-second, **no second LLM in the loop**.

[![Repo](https://img.shields.io/badge/repo-groundlens-181717?logo=github)](https://github.com/groundlens-dev/groundlens)
&nbsp;[![Stars](https://img.shields.io/github/stars/groundlens-dev/groundlens?label=%E2%98%85)](https://github.com/groundlens-dev/groundlens/stargazers)

`groundlens` · [`benchmark`](https://github.com/groundlens-dev/grounding-benchmark) · [`mcp`](https://github.com/groundlens-dev/groundlens-mcp) · [`cookbook`](https://github.com/groundlens-dev/Groundlens-Cookbook)

</td>
<td width="50%" valign="top">

### Otwin

**Physics-informed digital twins** with **calibrated uncertainty** for grid-scale energy storage and other physical systems. Port-Hamiltonian structure, leakage-free validation, CPU-first. White-box → grey-box.

[![Repo](https://img.shields.io/badge/repo-otwin-181717?logo=github)](https://github.com/groundlens-dev/otwin)
&nbsp;[![Stars](https://img.shields.io/github/stars/groundlens-dev/otwin?label=%E2%98%85)](https://github.com/groundlens-dev/otwin/stargazers)

Presented at **IEEE PES General Meeting 2026** (AI-powered Digital Twins for Grid-Scale Storage).

</td>
</tr>
</table>

<br>

##  Selected results

<div align="center">

<img src="https://raw.githubusercontent.com/groundlens-dev/otwin/main/assets/overview.png" width="780" alt="otwin workflow: choose a model structure, estimate, quantify uncertainty, validate" />

<table>
<tr>
<td align="center" width="50%">
<img src="https://raw.githubusercontent.com/groundlens-dev/otwin/main/examples/battery_soh/figures/01_hero_forecast.png" width="380" alt="Battery State-of-Health forecast with calibrated band" /><br>
<sub><b>Battery SoH</b> — the physics-informed hybrid tracks the real decay through end-of-life; a data-only model diverges.</sub>
</td>
<td align="center" width="50%">
<img src="https://raw.githubusercontent.com/groundlens-dev/otwin/main/examples/pumped_hydro/figures/pumped_hydro_energy.png" width="380" alt="Pumped-hydro round-trip efficiency validated against the closed form" /><br>
<sub><b>Pumped-hydro storage</b> — round-trip efficiency matches the closed form; energy conserved while idle.</sub>
</td>
</tr>
</table>

</div>

<br>

##  Featured

<div align="center">

<a href="POST_URL">
  <img src="assets/linkedin_post.png" width="420" alt="Featured LinkedIn post — 100k+ impressions" />
</a>

<sub> <b>100,000+ impressions</b> · <a href="POST_URL">read the post on LinkedIn →</a></sub>

</div>

<br>

##  About

Founder & Principal Engineer at Groundlens. Chemical engineer by training; fifteen years leading engineering and operations across regulated industries (process instrumentation, water technology, EPC), then moved full-time into the mathematics of modern AI. Today: open-source tools that make model outputs — from LLMs to physical digital twins — verifiable before they reach production.

Madrid ·  [javier@groundlens.dev](mailto:javier@groundlens.dev) ·  [groundlens.dev](https://groundlens.dev)

<div align="center">
<br>
<sub>Verification over capability.</sub>
</div>
