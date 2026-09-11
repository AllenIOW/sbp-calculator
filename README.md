# SBP Calculator

A calculator for the employee share option accounting charge under **IFRS 2**
and **FRS 102 Section 26**, together with the employer's National Insurance
provision and the deferred tax working.

**Try it: https://alleniow.github.io/sbp-calculator/**

It is being tested before wider use. If you prepare share-based payment
figures and are willing to run a real grant through it, I would value knowing
where it disagrees with your own working — that feedback is the point of
publishing it.

---

## What it covers

- The charge over the vesting period on the cumulative catch-up (true-up)
  method, including credits when expectations fall
- Service, non-market performance and market conditions, with the true-up
  asymmetry applied correctly — a failed market condition reverses nothing
- Graded vesting, accelerated by default (each tranche its own award), with
  the FRS 102 straight-line election available
- Black-Scholes valuation from your own inputs, with the full workings shown
- Modifications: repricing, beneficial and non-beneficial, and cancellation
- Employer's NIC, with applicability derived from the scheme type
- Deferred tax, including the split between profit or loss and equity

## Two things it does differently

**It shows its working.** No figure appears without its basis. Every row
expands to the arithmetic behind it; every schedule carries the inputs used,
the standard applied, the exact unrounded values, and a plain-language basis
of preparation written for someone reviewing the numbers rather than someone
reading the code.

**It will not guess your judgements.** Volatility, expected life, dividend
yield, share price at grant, the risk-free rate, tax and NIC rates and the
recoverability of a deferred tax asset are all yours to determine. The tool
refuses to default any of them and names the ones it is missing. Each comes
with guidance on what supports the number and where an auditor will press.

It also flags where it is uncertain rather than hiding it — the interpretations
it had to make are listed in every result, with the ones needing review against
the standard marked.

## Your figures stay with you

Everything is calculated in your browser. Nothing is uploaded, there is no
account, and there is no server behind this. Closing the tab discards the
data unless you have saved it yourself.

## Please read before relying on anything

- **This is not audited software** and it produces no filing. Treat every
  figure as a draft for review.
- **Equity-settled awards only.** Cash-settled awards (phantom options, SARs)
  are not yet supported.
- **The FRS 102 deferred tax treatment is applied by analogy to IAS 12** and
  is marked do-not-rely-until-verified. Section 29 is built on timing
  differences, and that working needs checking against the current text
  before it goes anywhere near statutory accounts.
- Some standard and statutory paragraph references were written from memory
  and are flagged for verification within the tool.

## If a number looks wrong

That is the most useful thing you can report. In the tool, open
**Scheme file → Export → Scheme file**, then save or copy it and send it over
with what you expected the figure to be and why. That file contains exactly
the inputs that produced what you saw, so the result can be reproduced rather
than guessed at.

Send it to me on
[LinkedIn](https://www.linkedin.com/in/jamie-allen-67308438), which is the
easiest way to reach me.

## About this repository

This holds the **built tool only** — a single self-contained HTML file. The
source, tests and design notes are not published here.

Engine version 0.2.0.

---

Built by Jamie Allen —
[linkedin.com/in/jamie-allen-67308438](https://www.linkedin.com/in/jamie-allen-67308438)

© Jamie Allen. All rights reserved. No licence is granted to copy, modify or
redistribute this tool.
