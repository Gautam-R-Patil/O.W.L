<div align="center">

# O.W.L

**The measurement instrument. TRUSCOR's hands and eyes on real computers.**

<p>
  <img src="https://img.shields.io/badge/STATUS-CLOSED%20SOURCE-172B4D?style=for-the-badge" alt="Closed source" />
  <img src="https://img.shields.io/badge/OPERATES-BROWSER%20%7C%20DESKTOP%20%7C%20SHELL-2EAD33?style=for-the-badge" alt="Operates environments" />
  <img src="https://img.shields.io/badge/FORMAT-.sova%20OPEN-00B8D9?style=for-the-badge" alt="Open format" />
  <a href="https://truscor.org"><img src="https://img.shields.io/badge/TRUSCOR-PROJECT%20HOME-0B8793?style=for-the-badge" alt="TRUSCOR" /></a>
</p>

</div>

---

## An agent's own report is not evidence

Ask an AI agent what it did and it will tell you. It will tell you it sent the
email, applied the refund, deleted the row, closed the ticket. Sometimes that
is true. Sometimes the call returned success and nothing happened. Sometimes
something else happened.

Every evaluation that trusts the agent's account of itself inherits that gap.

**O.W.L closes it by going and looking.**

## What it does

- **Operates test environments** — browsers, desktops and terminals, driven for real.
- **Observes what actually happened** and compares it against what the AI claimed.
- **Records signed evidence**, with a deliberate separation: *the action returned* is stored apart from *the intended effect occurred*. Those are different facts and collapsing them is how bad evaluations happen.
- **Replays findings** so they can be reproduced and checked by someone else.

Everything it writes lands in the open `.sova` format, so the measurement is
portable and inspectable rather than locked in a vendor report.

## Where it sits in the stack

| Layer | Role |
|---|---|
| **O.W.L** | Measures what happened on the machine |
| [SOVA Engine](https://github.com/TRUSCOR/SOVA-Engine) | Tests AI products, using O.W.L as its instrument |
| [SOVA Black Box](https://github.com/TRUSCOR/SOVA-Blackbox) | Records AI systems in production |
| [TAFAAR](https://github.com/TRUSCOR/TAFAAR) | Grades evidence into the TRUSCOR Rating (300-900) |
| [SOVA OSS](https://github.com/TRUSCOR/SOVA-OSS) | The free, open-source toolkit and the open `.sova` format |

*Sova* is the Serbian and Russian word for owl. The naming is not decoration —
the whole stack is built around watching rather than asking.

## About this repository

This repository holds public information and demo material for O.W.L.
**O.W.L's source code is private.**

## See the open layer run today

No model, API key or network needed:

```bash
git clone https://github.com/TRUSCOR/SOVA-OSS
cd SOVA-OSS
uv sync --locked
uv run sova demo sleeper
```

---

<div align="center">

© 2026 TRUSCOR Private Limited. All rights reserved.<br/>
<em>Where intelligence meets accountability.</em>

</div>
