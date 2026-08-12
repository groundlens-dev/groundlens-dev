<div align="center">
  
<img src="https://raw.githubusercontent.com/groundlens-dev/groundlens/main/docs/assets/Groundlens_01.png" width="22%">

# Groundlens: A proofreader for RAG answers

</div>

Give it an answer and the passages it was supposed to be written from. It hands
back the words those passages do not support, and next to each one, the closest
thing it found in your sources.

```
4.75%   support 0.00    nearest in policy.pdf#p3: '3.90%'
45      support 0.00    nearest in policy.pdf#p3: '30'
```

Two marks in a margin. What to do about them stays your call.

## Why we built it

We measured nine hallucination detectors across five benchmarks — 45
combinations — at the operating point production actually runs at: the
false-alarm rate you pay to catch 95% of hallucinations. The best of the 45 was
0.65. Two out of every three correct answers flagged for review.

Then we took one of those detectors and deleted the source documents before
running it again. It kept most of its ranking ability without them. Much of what
these systems detect is something other than grounding.

So we stopped trying to produce a verdict. There is no good one to give.
groundlens ships no threshold, no pass, no fail, no probability. It marks the
words and names the source span each one lost to, and leaves the judgement where
it already was — with the person who has to sign the document.

## How it reads

Two channels, because there are two kinds of content.

**Words are checked by meaning.** How close a word gets to anything in your
sources.

**Numbers are checked by arithmetic.** Parsed to a value, formatting normalised,
then present in the sources or absent. Nothing in between.

The second channel exists because the first one cannot do that job. Change
10,000 to 1,000 in a sentence and the meaning barely moves — but for a reviewer
at a bank, that digit is the entire document.

The figure for a whole answer is its **weakest** anchor, never the average. An
average is where one wrong number among sixty correct words goes to hide.

## Who it is for

A reviewer at a bank, an insurer, a law firm, a benefits agency — anywhere a
retrieval system drafts something a human has to sign. They have an answer,
three retrieved passages, and no time to read all four documents. That check
takes five minutes today and mostly gets skipped. With marks in the margin it
takes thirty seconds and gets done.

The human stays in the picture. The measurements above are what happens when you
try to remove them.

## The repositories

**[groundlens](https://github.com/groundlens-dev/groundlens)** — the library.
`pip install groundlens`, zero runtime dependencies, Apache-2.0.

**[groundlens-mcp](https://github.com/groundlens-dev/groundlens-mcp)** — the
connector, so an assistant can proofread an answer without leaving the
conversation.

**[groundlens.site](https://github.com/groundlens-dev/groundlens.site)** — the
source of [groundlens.dev](https://groundlens.dev).

## Start here

```bash
pip install "groundlens[encoder]"
groundlens read --answer answer.txt --context policy.pdf#p3=policy.txt
```

Thirty seconds and you will know whether this is useful to you. That is the
honest length of the pitch.

<div align="center">

[![License: Apache 2.0](https://img.shields.io/badge/License-apache--2.0-9a5416?style=for-the-badge)](LICENSE)


Groundlens is an independent open-source practice for trustworthy models. Maintained by [Javier Marin](https://www.linkedin.com/in/javiermarinvalenzuela/) · [javier@groundlens.dev](mailto:javier@groundlens.dev) · [groundlens.dev](https://groundlens.dev)
