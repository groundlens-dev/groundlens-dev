<div align="center">
  <img src="assets/Logo_groundlens_dev.png" alt="Groundlens" width="180">

# Groundlens: Open tools for verifying language models and agents outputs

[![Website](https://img.shields.io/badge/groundlens.dev-fc7604?style=for-the-badge&logo=astro&logoColor=white)](https://groundlens.dev)
[![Live demo](https://img.shields.io/badge/Hugging%20Face-Live%20demo-111111?style=for-the-badge&logo=huggingface&logoColor=FFD21E)](https://huggingface.co/spaces/groundlens/demo)
[![License: Apache 2.0](https://img.shields.io/badge/License-apache--2.0-9a5416?style=for-the-badge)](LICENSE)

</div>

##We turn "trust me" into "check me."

"Trust me" is not an answer when the stakes are real. So these tools do one thing, cheaply and the same way every time: they tell you whether a machine's answer actually came from the source it was supposed to use.

They read the geometry of the answer, not a second model's opinion, so the clear cases pass in milliseconds and only the doubtful ones cost you a person or a heavier check.

## How to use groundlens

- **Want to check whether an answer actually came from the document you gave the model?**
That is [**groundlens**](https://github.com/groundlens-dev/groundlens). Deterministic scores in milliseconds, no second model in the loop, the same result every time. It is the first stage: it decides what your expensive check has to look at.

- **Want that check running while you work, inside Claude Desktop, Cursor or Windsurf?**
[**groundlens-mcp**](https://github.com/groundlens-dev/groundlens-mcp) prints a reading under each answer as it arrives. It is a filter, not a judge, and every reading says so.

- **Have to show a supervisor that an answer followed a policy, with the evidence attached?**
[**groundlens-rules**](https://github.com/groundlens-dev/groundlens-rules) is hand-authored checklists that carry the text that triggered them. No model, no dependencies, and it never claims to be a measurement.

- **Want to know what these detectors actually measure, and where they stop working?**
[**grounding-benchmark**](https://github.com/groundlens-dev/grounding-benchmark) writes its false answers by hand rather than prompting a model for them, which is the case similarity-based detection finds hardest. Read the datasheet before quoting a number from it.

- **Want to see the components working together on a real pipeline?**
The [**Cookbook**](https://github.com/groundlens-dev/Groundlens-Cookbook) has executable notebooks: what each check settles, and what it hands on.

- **Curious about our numbers?**
Start with [what we withdrew](#what-we-withdrew) and the [confound table](#what-the-benchmarks-give-away-for-free), then the [benchmarks page](https://docs.groundlens.dev/benchmarks/results/). Every metric ships with its measured ceiling.

- **Want to try it without installing anything?**
The [live demo](https://huggingface.co/spaces/groundlens/demo).

- **Want to know the research where these methods como from?**
[**Research**](https://github.com/groundlens-dev/groundlens-dev/Research.md) 

--- 

If you are checking generated output in a pipeline that matters, and paying for it in tokens or in people, the problem is interesting to us.
Contact: javier@groundlens.dev](mailto:javier@groundlens.dev). 

---

## Contributing

Contributions are welcome across every repository. If you think a number here is wrong, open an issue with the reproduction — corrections get fixed and credited in the commit. Read [CONTRIBUTING.md](CONTRIBUTING.md) first.

## License

Everything here is Apache 2.0. See [LICENSE](LICENSE).

## About

Groundlens is an independent open-source practice for trustworthy modeling, working where applied geometry meets machine learning. Maintained by [Javier Marin](https://www.linkedin.com/in/javiermarinvalenzuela/) · [javier@groundlens.dev](mailto:javier@groundlens.dev) · [groundlens.dev](https://groundlens.dev)
