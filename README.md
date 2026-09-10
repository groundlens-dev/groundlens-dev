<div align="center">

<img src="https://raw.githubusercontent.com/groundlens-dev/groundlens/main/docs/assets/groundlens_header.png">

<br> 

<p align="center">
  <a href="https://github.com/groundlens-dev/groundlens/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-Apache--2.0-blue" alt="Apache-2.0"></a>
  <a href="https://www.bestpractices.dev/projects/13390"><img src="https://www.bestpractices.dev/projects/13390/badge" alt="OpenSSF Best Practices"></a>
  <a href="https://scorecard.dev/viewer/?uri=github.com/groundlens-dev/groundlens"><img src="https://api.securityscorecards.dev/projects/github.com/groundlens-dev/groundlens/badge" alt="OpenSSF Scorecard"></a>
  <a href="https://api.reuse.software/info/github.com/groundlens-dev/groundlens"><img src="https://api.reuse.software/badge/github.com/groundlens-dev/groundlens" alt="REUSE compliant"></a>
  <a href="https://slsa.dev"><img src="https://slsa.dev/images/gh-badge-level2.svg" alt="SLSA 2"></a>
</p>

<br>

## The verification and evidence layer for AI.
</div>
<br>

GroundLens is verification infrastructure for AI systems in production. It
checks what an AI system produced, decides what to do with it under
policies you control, and issues a signed evidence record that customers,
auditors and regulators can verify independently. It runs inside your
environment, on your outputs, without access to your models, prompts or
architecture.

<br>

## Why a verification layer

AI systems now produce factual claims, recommendations and decisions that
organisations are accountable for. The tooling around them has matured in
three directions: evaluation before release, observability in production,
and guardrails on inputs and outputs. None of the three produces what an
accountable organisation needs when a decision is questioned: proof that
this specific output was checked, with which methods, under which rules,
and that the check can be reproduced.

GroundLens is that missing layer. It is not a model, a benchmark or a
dashboard. It is the infrastructure through which verification is
performed, governed and evidenced, in the same sense that a payment
processor is infrastructure for transactions or an identity provider is
infrastructure for authentication: a stable contract, shared across
applications, independent of any one of them.

## What the platform provides

- [x] **Verification engine.** One pipeline, implemented once in Rust and exposed
to Python, the command line and, on the roadmap, HTTP and WebAssembly: an
output is decomposed into claims, every admitted verifier examines the
claims and returns evidence, a policy interprets the evidence, and the
whole chain is sealed into a record. The same input, policy and models
produce the same record on any machine; this is tested on Linux, macOS and
Windows on every commit.

- [x] **Verifiers.** Independent methods under one contract. Each verifier
returns evidence, never a verdict, and declares what it guarantees: exact,
reproducible within a stated tolerance, or non-deterministic. The platform
ships exact numeric verification (numbers, currencies, percentages and
physical units across locales), symbolic rules, and lexical grounding on a
pinned multilingual encoder. Entailment, semantic, geometric and
model-based verifiers, and adapters for third-party detectors, follow on
the roadmap. Existing verification libraries are not competitors of this
layer; they are candidates to run inside it.

- [x] **Policies.** Decisions are made by versioned, hashed policy documents,
not by application code. A policy states which verifiers are required,
recommended, optional or forbidden, which determinism class is allowed to
decide, the thresholds and guard bands that apply, how disagreements and
unresolved claims are handled, and which governance or regulatory controls
each outcome concerns. Two organisations can apply different policies to
the same evidence and both are correct; that is where risk appetite lives.

- [x] **Evidence records.** Every verification produces an append-only,
hash-chained, Ed25519-signed record: input hashes, verifier and model
hashes, the evidence, the policy and its hash, the decision, the
regulatory mapping, and the link to the previous record. A log of records
is an audit trail that can be handed over as a file and verified offline
by anyone, with no trust in the party that produced it.

- [x] **Bundles.** Models, tokenizers, calibrations, rules and policies travel
as versioned bundles with a manifest of hashes. A bundle is verified
artefact by artefact before it runs, is named by hash in every record, and
can be installed by hand in an isolated environment. The engine itself
never opens a network connection.

<br>

## Built for

- [x] Teams that ship AI outputs into workflows where someone will ask for.
- [x] AI vendors and system integrators serving regulated customers,
platforms whose answers feed financial, legal, medical or operational
decisions.
- [x] Organisations preparing conformity and record-keeping
evidence under the EU AI Act and comparable frameworks. GroundLens works
on outputs and evidence alone, so independent verification is possible
without disclosing how the system under review is built.

<br>

## Principles

A verifier produces evidence, not truth. The policy decides, and the
policy is yours. Deterministic where possible, reproducible where
required, explicit provenance when neither is. Local execution, no
runtime dependencies, no network. Independence from the system being
verified, because a check that depends on the thing it checks is not a
check.

<br>

## Project scope

The engine, the verifiers, the policy language, the record format and the
command line are open source under Apache-2.0, and will remain so: the
record format only earns trust if anyone can inspect the code that
produces and verifies it. 

GroundLens non-open source offerings cover
verification at production scale: calibration on your data, evidence
packages for procurement and conformity files, maintained policies and
regulatory mappings, specialised verifiers, and private deployment.

<br>

<div align="center">
  
[groundlens](https://github.com/groundlens-dev/groundlens) | [README](https://github.com/groundlens-dev/groundlens#readme) | [FAQ](https://github.com/groundlens-dev/groundlens/blob/main/FAQ.md) | [Roadmap](https://github.com/groundlens-dev/groundlens/blob/main/ROADMAP.md) | [Changelog](https://github.com/groundlens-dev/groundlens/blob/main/CHANGELOG.md) | [PyPI](https://pypi.org/project/groundlens/) | [groundlens.dev](https://groundlens.dev)

<br>
<sub>GroundLens (2026) · javier@jgroundlens.dev</sub>
</div>
