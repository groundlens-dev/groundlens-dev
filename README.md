<div align="center">

<img src="assets/groundlens_diagram.png" alt="The LLM answer and its passages go through GroundLens first, then an LLM judge, then human review. A policy decides, and every check leaves a signed record.">

<br>

# Guardrails for LLM answers

<a href="https://pypi.org/project/groundlens/"><img src="https://img.shields.io/pypi/v/groundlens?color=1a4fd6" alt="PyPI"></a>
<a href="https://github.com/groundlens-dev/groundlens/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-Apache--2.0-blue" alt="Apache-2.0"></a>
<a href="https://scorecard.dev/viewer/?uri=github.com/groundlens-dev/groundlens"><img src="https://api.securityscorecards.dev/projects/github.com/groundlens-dev/groundlens/badge" alt="OpenSSF Scorecard"></a>
<a href="https://slsa.dev"><img src="https://slsa.dev/images/gh-badge-level3.svg" alt="SLSA 3"></a>

</div>

<br>

<p align="center">GroundLens checks an LLM answer</p>
<p align="center">against its sources without a model,</p>
<p align="center">decides PASS, REVIEW or FAIL under </p>
<p align="center">your policy, and keeps a signed record.</p>


## Why Groundlens

LLM answers now carry figures that organisations act on: amounts, rates,
dates, limits. The tools around them grew in three directions: evaluation
before release, observability in production, and filters on what goes in and
out. None of them answers the question asked when a decision is challenged:
was this answer checked, how, under which rule, and can you prove it?

GroundLens answers it for every answer. The checks are exact, so the same
answer gets the same result on any machine. The policy that decides is a file
you own. The record of each decision is signed, chained to the one before,
and checkable by anyone without our software.

<br>

## How it works

- **A check produces evidence, not truth.** Your policy decides what it means.
- **Exact first.** No model where arithmetic will do. A model, if you add one, can escalate an answer, never pass it.
- **Nothing that failed can pass.** A check that could not run, or a record that could not be stored, is never a PASS.
- **Runs where you run.** In your process, with no network, no account and no access to your models or prompts.
- **Open, so it can be trusted.** A record is only evidence if anyone can inspect the code that writes and verifies it.

<br>

## Project content

| | |
|---|---|
| **[groundlens](https://github.com/groundlens-dev/groundlens)** | The package and the engine. Start here: `pip install groundlens` |
| **[Documentation](https://groundlens.readthedocs.io)** | Guides, policies, integrations and the full reference |
| **[groundlens.dev](https://groundlens.dev)** | What it does, what it catches, and how it compares with other tools |
| **MCP registry** | `io.github.groundlens-dev/groundlens`, for agents that check their own answers |

<br>

## Open source, and beyond

The engine, the checks, the policies, the connectors, the command line and
the MCP server are Apache-2.0, and will stay so. For teams that need more:
measurement on your own data, evidence packages for procurement and
conformity files, maintained policies and regulatory mappings, and private
deployment. Write to javier@groundlens.dev.

<br>

<div align="center">
<sub>Copyright GroundLens 2026</sub>
</div>
