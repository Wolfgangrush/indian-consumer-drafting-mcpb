# Wolfgang Rush — Indian Consumer Forum Drafting

**MCPB Desktop Extension** for drafting pleadings before District / State / National Consumer Disputes Redressal Commissions under the Consumer Protection Act 2019.

CPA 2019-compliant. Designed for Indian advocates using **Claude Desktop App**. Local-execution. Zero data collection.

> *Also available as a Claude Code Plugin:* *[github.com/Wolfgangrush/indian-consumer-drafting](https://github.com/Wolfgangrush/indian-consumer-drafting)*

---

## Case types (10)

### Original complaints

| Forum | Statutory anchor |
|---|---|
| District Consumer Forum | CPA 2019 Section 35 |
| State Consumer Commission | CPA 2019 Section 47 |
| NCDRC | CPA 2019 Section 58 |
| Medical-negligence | Jacob Mathew / Bolam framework |
| Product-liability | CPA 2019 Section 83 |
| Unfair-trade-practice | CPA 2019 |

### Appellate / revisional / execution

| Case type | Statutory anchor |
|---|---|
| Appeal District → State | CPA 2019 Section 41 |
| Appeal State → NCDRC | CPA 2019 Section 51 |
| Revisional application | CPA 2019 Section 67 |
| Execution application | CPA 2019 Section 71 |

## Install

1. Claude Desktop App → **Settings → Extensions → Install Extension**
2. Select `wolfgang-indian-consumer-drafting.mcpb`
3. Enable

## System requirements

Claude Desktop App ≥ 0.10.0 · Python ≥ 3.10 · `pandoc` · `pdftotext` (optional)

## Tools

`list_case_types` · `get_case_type_format` · `get_agent_instructions` · `get_pleading_base` · `read_case_folder` · `save_draft_as_docx`

## Privacy

Zero data collection. Three-layer privacy firewall. Canonical policy: **<https://wolfgangrush.github.io/privacy/>**


## ⚠️ AI verification disclaimer · 🔒 Pseudonymisation procedure

> **⚠️ AI can make mistakes — please verify the information before filing.**
> Every draft produced by this connector is a STARTING POINT. The Verifier
> agent runs an anti-hallucination firewall and the Overseer agent runs an
> opposing-counsel review, but neither replaces an advocate's independent
> verification of statutory references, citation accuracy, factual fidelity,
> and Registry-formatting compliance with the user's High Court / forum.
> The advocate filing the pleading remains responsible for the contents.
>
> **🔒 Protected by pseudonymisation procedure.** The Reader agent applies a
> domain-specific privacy firewall as the first step of the pipeline — party
> names, addresses, identifying numbers (FIR / CR / Crime / Suit / Diary /
> SLP / lower-court case numbers), PAN / Aadhaar references, financial
> figures, witness names, and statutory-notice references are substituted
> with structural placeholders BEFORE any downstream agent sees the facts.
> The Drafter, Verifier, Refiner, and Overseer agents process placeholders
> only. Real values are re-substituted at the final docx render step on the
> user's local machine. No real identifying data leaves the case folder.

## License

MIT.

## Publisher

**Rushikesh R. Mahajan**, Advocate, Bombay HC Nagpur, publishing as **Wolfgang Rush**. advrushikeshravindramahajan@gmail.com

## Source

<https://github.com/Wolfgangrush/indian-consumer-drafting-mcpb>
