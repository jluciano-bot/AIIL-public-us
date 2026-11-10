<!-- aiil-logo-header:start -->
<p align="left"><img src="website/Blue%20Hexagon%20Temple%20Logo.png" alt="AIIL - Artificial Intelligence Infrastructure Library" height="72"></p>
<!-- aiil-logo-header:end -->

# AIIL — Licensing

Status: **Draft, chosen by the owner on 2026-11-04. Not yet reviewed by a lawyer.** This is not legal advice.

Copyright (c) 2026 Jose Da Silva.

## What licence applies to what

| Material | Where | Licence | File |
|---|---|---|---|
| Content: framework, processes, pillars, glossary, governance, guides, methodology, whitepaper, specification (includes `framework/tl-ai/`, imported 2026-11-09 from the owner's own repository, which was Apache 2.0 there; the owner is the author and relicensed it) | `docs/`, `framework/`, `governance/`, `assessments/`, `research/`, `aiil-analyzer/*.md`, `mcp/*.md` | **Creative Commons Attribution 4.0 International (CC BY 4.0)** | `LICENSE-CONTENT-CC-BY-4.0.txt` |
| Code: scoring engine, data file, report code, tests | `website/*.js`, `aiil-analyzer/tests/` | **Apache License 2.0** | `LICENSE` |
| Name "AIIL", logos, hexagon, animated intro, social cards | `website/*.png`, `website/*.mp4`, `social/` | **Not licensed.** See "Trademark and brand" below | — |

## What you can do (content and code)

- Use, copy, share, translate and adapt the material, including for commercial work such as consulting and training.
- Credit is required. For the content, give the author's name, link to the licence, and say if you changed it. For the code, keep the copyright notice and the Apache licence text.
- Apache 2.0 also gives a patent licence for the code.

## Trademark and brand

The CC BY and Apache licences cover the text and the code. They **do not** give any right to the name "AIIL", the logos, or the visual identity.

- You may say your work is "based on the AIIL framework" or "aligned with AIIL", with credit.
- You may **not** present something as an official AIIL certification, accreditation, course, or exam, or use the AIIL name or logos in a way that suggests the author endorses you.
- Official AIIL training and certification, if offered, will be defined by the author separately.

The name "AIIL" is **not registered** as a trademark (owner decision, 2026-11-04). A registration search by an attorney or agent is still pending. Until that is done, this section states the author's intent and has limited legal force.

## Before publishing

- [ ] Lawyer review of this file and the choice of licences.
- [x] Add an SPDX line (`SPDX-License-Identifier: Apache-2.0`) at the top of each code file (done 2026-11-04, 7 files).
- [ ] Add a short "License" section to `README.md` linking here (done).
- [x] Logos and watermark: **owner decision 2026-11-04 (corrected).** Every document and every site page must show the AIIL logo and a faint watermark. What is not offered is the loose logo file (for example `logo.png`) for others to reuse: it is covered by the brand rule above, not by CC BY or Apache. Logos inside `website/aiil-brand.js` are brand assets inside Apache-licensed code; the Apache licence covers the code only.
