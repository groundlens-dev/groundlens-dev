<div align="center">
  
# Groundlens: Geometric methods for trustworthy models

<p>
An open-source practice for <b>trustworthy modeling</b> — making the outputs of both AI systems and physical systems verifiable.<br>
</p>

[![Website](https://img.shields.io/badge/groundlens.dev-fc7604?style=for-the-badge&logo=astro&logoColor=white)](https://groundlens.dev)
[![Live demo](https://img.shields.io/badge/Hugging%20Face-Live%20demo-111111?style=for-the-badge&logo=huggingface&logoColor=FFD21E)](https://huggingface.co/spaces/groundlens/demo)
[![License: Apache](https://img.shields.io/badge/License-apache--2.0-9a5416?style=for-the-badge)](LICENSE)

<br>

</div>

---

[1. Mission](#mission) 

[2. Projects](#projects)

[3. Research](#research)

[4. Featured](#featured)

[5. Contributing](#contributing)

[6. License](#license)

[7. About](#about)

---

## Mission
<div align="center">
  
*We turn "trust me" into "check me.*

</div>

AI is fluent, and fluency hides error. A language model that sounds right and a black-box predictor that fits the data can both be confidently wrong — and neither can prove otherwise. Groundlens builds the layer that checks: every claim measured against ground truth you can inspect — the source it cited, the physics it must obey, the geometry of its own representations. No second opaque model casting a vote. Deterministic, reproducible, the same verdict every time.
**If it can't be verified, it can't be trusted. So we make it verifiable.**

## Projects

<div align="center">
  
<img src="assets/groundlends_logo.png" height="120" alt="Groundlens" />

### Groundlens: the deterministic first stage for RAG and agent loops. </br> It decides what your LLM judge has to look at.

[![Repo](https://img.shields.io/badge/repo-groundlens--dev/groundlens-181717?style=flat&logo=github)](https://github.com/groundlens-dev/groundlens)
&nbsp;[![Stars](https://img.shields.io/github/stars/groundlens-dev/groundlens?label=%E2%98%85)](https://github.com/groundlens-dev/groundlens/stargazers)

[`groundlens`](https://github.com/groundlens-dev/groundlens) · [`grounding-benchmark`](https://github.com/groundlens-dev/grounding-benchmark) · [`groundlens-mcp`](https://github.com/groundlens-dev/groundlens-mcp) · [`Groundlens-Cookbook`](https://github.com/groundlens-dev/Groundlens-Cookbook)

</div>

Geometric grounding and hallucination triage for production LLMs in regulated industries. It ranks responses by how faithfully they reflect their sources — **deterministic scores, sub-second, no second LLM in the loop** — so the ones that earned trust pass and the rest go to human review.

<div align="center">

[![Try the live demo](https://img.shields.io/badge/Hugging%20Face-Try%20the%20live%20demo-111111?style=for-the-badge&logo=huggingface&logoColor=FFD21E)](https://huggingface.co/spaces/groundlens/demo)

</div>

> [!TIP]  
> Run grounding verification in your browser — no install.


### ndt — Neural Dimensionality Tracker

High-frequency monitoring of how a neural network's internal representations evolve during training. It tracks representational **dimensionality** across MLPs, CNNs, Transformers and Vision Transformers, and flags discrete phase transitions (jumps) — the same DNA as Groundlens: reading the *geometry of representations* to see what a model is actually doing. Three lines to instrument any PyTorch model.

<div align="center">

[![Repo](https://img.shields.io/badge/repo-groundlens--dev/ndt-181717?style=flat&logo=github)](https://github.com/groundlens-dev/ndt)
&nbsp;[![Stars](https://img.shields.io/github/stars/groundlens-dev/ndt?label=%E2%98%85)](https://github.com/groundlens-dev/ndt/stargazers)
&nbsp;[![PyPI](https://img.shields.io/pypi/v/ndtracker?label=ndtracker)](https://pypi.org/project/ndtracker/)

</div>

```bash
pip install ndtracker
```

## Research

Groundlens is built on peer-reviewed research. Selected publications:

| Year | Publication | Venue / link |
|---|---|---|
| 2026 | Rotational Dynamics of Factual Constraint Processing | [arXiv:2603.13259](https://arxiv.org/abs/2603.13259) |
| 2026 | A Geometric Taxonomy of Hallucinations | [arXiv:2602.13224](https://arxiv.org/abs/2602.13224) |
| 2025 | Semantic Grounding Index (SGI) | [arXiv:2512.13771](https://arxiv.org/abs/2512.13771) |
| 2025 | Hamiltonian Neural Networks for Out-of-Time Credit Scoring - accepted (peer-reviewed), IEEE DSAA 2025| [arXiv:2410.10182](https://arxiv.org/abs/2410.10182)|
| 2024 | Optimizing AI Reasoning: A Hamiltonian Dynamics Approach to Multi-Hop QA | [arXiv:2410.04415](https://arxiv.org/abs/2410.04415) |

<div align="center">

[![Full publication list — Google Scholar](https://img.shields.io/badge/Full%20list-Google%20Scholar-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white)](https://scholar.google.es/citations?user=cqDaAlEAAAAJ&hl=es)

</div>

<br>

## Featured

<div align="center">

<a href="https://www.linkedin.com/feed/update/urn:li:share:7407335601592741888/">
  <img src="assets/Linkedin_post.png" width="400" alt="Featured LinkedIn post — 100,000+ impressions" />
</a>

<sub><b>100,000+ impressions</b> · <a href="https://www.linkedin.com/feed/update/urn:li:share:7407335601592741888/">read it on LinkedIn</a></sub>

</div>

<br>


## Contributing

Contributions are welcome across all Groundlens repositories. Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening an issue or pull request.

## License

All Groundlens open-source projects are released under the **APACHE 2.0**. See [LICENSE](LICENSE).

## About

**Groundlens** is an independent open-source practice for trustworthy modeling, working at the intersection of applied geometry, physics, and machine learning. Its two lines — Groundlens (LLM verification) and Otwin (physics-informed digital twins) — share a single goal: outputs you can audit before they reach production.

Maintained by [Javier Marin](https://www.linkedin.com/in/javiermarinvalenzuela/) | [javier@groundlens.dev](mailto:javier@groundlens.dev) | [groundlens.dev](https://groundlens.dev)

<div align="center">
  
[![Donation](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-%5E%5E-green?style=flat&logo=undertale&logoColor=green&color=white)](https://github.com/sponsors/armync)

</div>



