<div align="center">

# O.W.L

**TRUSCOR's measurement instrument: its hands and eyes on real computers.**

Closed source · used by SOVA Engine, SOVA Black Box and licensed measurers · by [TRUSCOR](https://truscor.org)

</div>

---

## What it does

An AI agent's own report of what it did isn't evidence. O.W.L checks.

- **Operates test environments:** browsers, desktops and terminals.
- **Observes what really happened** and compares it with what the AI claimed.
- **Records signed evidence:** every action records "the action returned" separately from "the intended effect happened", in the open `.sova` format.
- **Replays findings** so they can be reproduced and checked.

## Where it fits in the SOVA stack

| Part | Role |
|---|---|
| **O.W.L** | Measures what happened on the machine |
| [SOVA Engine](https://github.com/TRUSCOR/SOVA-Engine) | Tests AI products using O.W.L |
| [SOVA Black Box](https://github.com/TRUSCOR/SOVA-Blackbox) | Records AI systems in production |
| [TAFAAR](https://github.com/TRUSCOR/TAFAAR) | Grades evidence into the TRUSCOR Rating |
| [SOVA OSS](https://github.com/TRUSCOR/SOVA-OSS) | The free, open-source toolkit and the open `.sova` format |

## About this repository

This repository holds public information and demo material for O.W.L. **O.W.L's source code is private.**

## See the open part run today

```bash
git clone https://github.com/TRUSCOR/SOVA-OSS
cd SOVA-OSS
uv sync --locked
uv run sova demo sleeper
```

---

© 2026 TRUSCOR Private Limited. All rights reserved.
