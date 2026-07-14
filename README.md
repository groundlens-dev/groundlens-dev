<div align="center">
  
# :triangular_ruler: Groundlens: Geometric methods for trustworthy models

<p>
An open-source practice for <b>trustworthy modeling</b> — making the outputs of both AI systems and physical systems verifiable.<br>
</p>

[![Website](https://img.shields.io/badge/groundlens.dev-fc7604?style=for-the-badge&logo=astro&logoColor=white)](https://groundlens.dev)
[![Live demo](https://img.shields.io/badge/Hugging%20Face-Live%20demo-111111?style=for-the-badge&logo=huggingface&logoColor=FFD21E)](https://huggingface.co/spaces/groundlens/demo)
[![License: Apache](https://img.shields.io/badge/License-apache--2.0-9a5416?style=for-the-badge)](LICENSE)

<br>

</div>

---
# Table of Contents

  - [Mission](#mission) 

  - [Projects](#projects)
      - [:traffic_light: Groundlens](#groundlens)
      - [:electric_plug: Groundelens MCP](#groundlens-mcp)
      - [:signal_strength: Groundelens Benchmark](#groundlensbenchmark)
      - [:microscope: Neural Dimensionality Tracker](#neuraldimensionalitytracker)

  - [Research](#research)

  - [Contributing](#contributing)

  - [License](#license)

  - [About](#about)


<br>


## Mission
  
*We turn "trust me" into "check me.*


AI is fluent, and fluency hides error. A language model that sounds right and a black-box predictor that fits the data can both be confidently wrong — and neither can prove otherwise. Groundlens builds the layer that checks: every claim measured against ground truth you can inspect — the source it cited, the physics it must obey, the geometry of its own representations. No second opaque model casting a vote. Deterministic, reproducible, the same verdict every time.
**If it can't be verified, it can't be trusted. So we make it verifiable.**

<br>


## Projects


### :traffic_light: Groundlens
[![Repo](https://img.shields.io/badge/repo-groundlens--dev/groundlens-181717?style=flat&logo=github)](https://github.com/groundlens-dev/groundlens)
&nbsp;


The deterministic first stage for RAG and agent loops. It decides what your LLM judge has to look at.

Geometric grounding and hallucination triage for production LLMs in regulated industries. It ranks responses by how faithfully they reflect their sources — **deterministic scores, sub-second, no second LLM in the loop** — so the ones that earned trust pass and the rest go to human review.

[![Try the live demo](https://img.shields.io/badge/Hugging%20Face-Try%20the%20live%20demo-111111?style=for-the-badge&logo=huggingface&logoColor=FFD21E)](https://huggingface.co/spaces/groundlens/demo)

> [!TIP]  
> Run grounding verification in your browser — no install.


### :electric_plug: Groundlens-MCP
[![Repo](https://img.shields.io/badge/repo-groundlens--dev/groundlens-181717?style=flat&logo=github)](https://github.com/groundlens-dev/groundlens-mcp)&nbsp;


MCP server for groundlens — a deterministic first-stage grounding check for Claude Desktop, Cursor, Windsurf, and any MCP-compatible client. It checks whether an answer was drawn from its source, in milliseconds, with no model in the scoring path. Same inputs → same scores, every time.

> [!NOTE]
> It is a filter, not a judge. It has a characterized blind spot, and every check says so.

| Tool | Install|
|------|---------------|
| Cursor | [![Install in Cursor](https://img.shields.io/badge/Cursor-Add_MCP-000000?style=flat-square&logo=cursor&logoColor=white)](https://cursor.com/install-mcp?name=groundlens&config=eyJjb21tYW5kIjoidXZ4IiwiYXJncyI6WyJncm91bmRsZW5zLW1jcCJdfQ%3D%3D)|
| VS Code | [![Install in VS Code](https://img.shields.io/badge/VS_Code-Add_MCP-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://insiders.vscode.dev/redirect/mcp/install?name=groundlens&config=%7B%22command%22%3A%22uvx%22%2C%22args%22%3A%5B%22groundlens-mcp%22%5D%7D)|
| VS Code Insiders |  [![Install in VS Code Insiders](https://img.shields.io/badge/VS_Code_Insiders-Add_MCP-24bfa5?style=flat-square&logo=visualstudiocode&logoColor=white)](https://insiders.vscode.dev/redirect/mcp/install?name=groundlens&config=%7B%22command%22%3A%22uvx%22%2C%22args%22%3A%5B%22groundlens-mcp%22%5D%7D&quality=insiders) |


### :signal_strength: Groundelens Benchmark
[![Repo](https://img.shields.io/badge/repo-groundlens--dev/groundlens-181717?style=flat&logo=github)](https://github.com/groundlens-dev/groundlens-benchmark)&nbsp;


#### A Methodology for Building Human-Confabulated Hallucination Benchmarks

Almost every hallucination benchmark generates its false content by prompting an LLM. This one does not. A non-expert writes the false response from memory, without consulting any source, producing a confabulation in the neuropsychological sense (Berlyne, 1972): confident, domain-appropriate, and wrong.

The consequence is the finding that motivates the dataset. Embedding-similarity detectors that reach 88–97% on LLM-generated benchmarks fall to 69–78% on these human confabulations, and on the in-register cases (template-structured domains) they fall to chance. The false responses stay inside the distributional register of their domain, and a detector that scores grounding by embedding similarity cannot tell them apart from correct answers. This is a property of the embedding geometry, not a tuning gap.

This dataset is the evidence base for that result. The controlled study built on it, the register-distance dose-response, the authorship shortcut, and the geometric ceiling, is reported in The Register Wall: What Similarity-Based Hallucination Detectors Actually Measure (Marín, 2026; under review).


### :microscope: Neural Dimensionality Tracker
[![Repo](https://img.shields.io/badge/repo-groundlens--dev/ndt-181717?style=flat&logo=github)](https://github.com/groundlens-dev/ndt)
&nbsp;


High-frequency monitoring of how a neural network's internal representations evolve during training. It tracks representational **dimensionality** across MLPs, CNNs, Transformers and Vision Transformers, and flags discrete phase transitions (jumps) — the same DNA as Groundlens: reading the *geometry of representations* to see what a model is actually doing. Three lines to instrument any PyTorch model.

```bash
pip install ndtracker
```

<br>


## :book: Research

Groundlens is built on peer-reviewed research. Selected publications:

| Year | Publication | Link |
|---|---|---|
| 2026 | Rotational Dynamics of Factual Constraint Processing | [arXiv:2603.13259](https://arxiv.org/abs/2603.13259) |
| 2026 | A Geometric Taxonomy of Hallucinations | [arXiv:2602.13224](https://arxiv.org/abs/2602.13224) |
| 2025 | Semantic Grounding Index (SGI) | [arXiv:2512.13771](https://arxiv.org/abs/2512.13771) |


[![Full publication list — Google Scholar](https://img.shields.io/badge/Full%20list-Google%20Scholar-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white)](https://scholar.google.es/citations?user=cqDaAlEAAAAJ&hl=es)

<br>

## Contributing

Contributions are welcome across all Groundlens repositories. Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening an issue or pull request.

<br>

## License

All Groundlens open-source projects are released under the **APACHE 2.0**. See [LICENSE](LICENSE).

<br>

## About

**Groundlens** is an independent open-source practice for trustworthy modeling, working at the intersection of applied geometry, physics, and machine learning. Its two lines — Groundlens (LLM verification) and Otwin (physics-informed digital twins) — share a single goal: outputs you can audit before they reach production.

Maintained by [Javier Marin](https://www.linkedin.com/in/javiermarinvalenzuela/) | [javier@groundlens.dev](mailto:javier@groundlens.dev) | [groundlens.dev](https://groundlens.dev)

<div align="center">
  
[![Donation](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-%5E%5E-green?style=flat&logo=undertale&logoColor=green&color=white)](https://github.com/sponsors/armync)

</div>



