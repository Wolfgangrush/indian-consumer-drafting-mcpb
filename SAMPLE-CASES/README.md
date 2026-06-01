# Sample Cases — Reviewer Examples

Three anonymised Consumer Forum fact patterns. All party names are placeholders.

## Example 1 — District Forum complaint (Section 35) for delayed apartment possession

> *"Draft a consumer complaint before the District Consumer Forum at [DISTRICT-X] under Section 35 CPA 2019 against [BUILDER] for delayed possession of apartment booked 2022-06-15 for ₹[SUM-A], possession promised by 2024-12-31, still not delivered. Interest on deposit + compensation + costs claimed. Pecuniary jurisdiction under ₹50 lakhs."*

Tool sequence: list_case_types → get_case_type_format("district-commission-complaint-section-35") → get_pleading_base → draft → save_draft_as_docx

## Example 2 — Medical-negligence complaint (Jacob Mathew framework)

> *"Draft a medical-negligence complaint before the State Consumer Commission against [HOSPITAL] and [DR-X]. Patient [P] underwent [PROCEDURE] on 2025-03-10; post-operative complications arising from deviation from standard of care (improper sterilisation protocol, delayed escalation). Jacob Mathew / Bolam standard pleaded. Quantum: ₹[SUM-X] compensation + ₹[SUM-Y] medical expenses + costs."*

Tool sequence: list_case_types → get_case_type_format("medical-negligence-complaint") → get_pleading_base → draft → save_draft_as_docx

## Example 3 — Appeal Section 41 from District Forum to State Commission

> *"Draft an appeal under Section 41 CPA 2019 to the State Consumer Commission against the District Forum order dated 2026-01-15 in Complaint No. [CC-N]/2025. Grounds: District Forum failed to consider documentary evidence of deficiency at Exhibit P-5, misapplied limitation provisions under Section 69, computed compensation without reference to Sarla Verma multiplier framework. Prayer: setting aside + remand or enhanced compensation."*

Tool sequence: list_case_types → get_case_type_format("consumer-appeal-section-41-district-to-state") → get_pleading_base → draft → save_draft_as_docx

## Notes for the reviewer

- Placeholders only (`[BUILDER]`, `[HOSPITAL]`, `[DR-X]`, `[P]`, `[SUM-A]`, `[CC-N]`, etc.). No real client data.
- No external API keys / accounts required.
- `save_draft_as_docx` requires `pandoc`.

---

## Synthetic case folder for Anthropic reviewer

A fully-fictional, AAAK-pseudonymised case folder is bundled at:

`SAMPLE-CASES/synthetic-district-commission-delayed-possession/`

It contains 4 source documents (.docx) plus a `case-facts-background.md` narrative.

**To exercise the pipeline end-to-end**, point `read_case_folder(path)` at this folder and follow the orchestration script returned by `get_agent_instructions()`. The Reader stage will extract facts, the Format stage will load the case-type SKILL.md template, and the remaining four agents (Drafter → Verifier → Refiner → Overseer) will produce `final-draft.docx`.

All identifiers in the bundled documents are structural placeholders. The Pseudonymisation Gateway is therefore exercising against pre-pseudonymised content; reviewers seeking to test re-substitution may replace placeholders with their own fictional values before invoking the pipeline.

