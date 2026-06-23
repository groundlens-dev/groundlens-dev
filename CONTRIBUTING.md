# Contributing to Groundlens

Thank you for considering a contribution. Groundlens is an open-source practice for
trustworthy modeling, spanning two lines — **Groundlens** (LLM output verification) and
**Otwin** (physics-informed digital twins). Contributions are welcome across all
repositories in the [groundlens-dev](https://github.com/groundlens-dev) organization.

## Ways to contribute

- **Report a bug** — open an issue with a minimal, reproducible example.
- **Propose a feature** — open an issue describing the problem first, before the solution.
- **Improve documentation** — corrections and clarifications are always welcome.
- **Submit code** — fix a bug or implement an agreed feature via a pull request.

## Development setup

Each project documents its own setup in its repository. In general:

```bash
git clone https://github.com/groundlens-dev/<repo>.git
cd <repo>
pip install -e ".[dev]"     # or: uv pip install -e ".[dev]"
pytest                       # run the test suite
```

## Pull request guidelines

1. **Open an issue first** for anything beyond a small fix, so we can agree on scope.
2. **Keep changes focused** — one logical change per pull request.
3. **Add tests** for new behavior; do not reduce coverage.
4. **Pass the checks** — linting, formatting, and type checks must be green
   (projects use `ruff`, `black`, and `mypy`).
5. **Write clear commit messages** describing what changed and why.
6. **Update documentation** when behavior changes.

## Standards

- Be rigorous. Claims in code, docs, and figures must be reproducible from the repository.
- Report limitations plainly; do not overstate results.
- Match the existing style and naming conventions of the project you are editing.

## Code of Conduct

By participating you agree to uphold our [Code of Conduct](CODE_OF_CONDUCT.md).

## Questions

Open a discussion or issue, or reach out at <javier@groundlens.dev>.
