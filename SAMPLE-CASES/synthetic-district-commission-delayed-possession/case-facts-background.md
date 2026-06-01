# Case Facts Background — District Consumer Commission Section 35 complaint · delayed apartment possession

All party names, project names, monetary figures, RERA registration numbers, addresses, and ancillary dates are fictional placeholders.

## Parties

- **Complainant:** [Complainant-A], son of [Complainant-Father-Placeholder], residing at [Complainant-Address-Placeholder]. Salaried professional, sole Allottee of the apartment.
- **Opposite Party:** M/s [Builder-Company-Placeholder] Private Limited, CIN [Builder-CIN-Placeholder], having registered office at [Builder-Office-Placeholder]. The Promoter under the Agreement for Sale.

## Subject matter

- Apartment No. [Apartment-No-Placeholder] at [Project-Name-Placeholder] (RERA Registration No. [RERA-Registration-Placeholder]) in [Project-Location-Placeholder].
- Total agreed consideration: Rs. [Sum-A-Placeholder]/- (within District Commission pecuniary jurisdiction of < Rs. 50 lakh per Section 34 CPA 2019).
- Carpet area: [Carpet-Area-Placeholder] sq. ft.

## Contract terms

- Promised Possession Date: 31 December 2024 (Clause 7.1 of Agreement)
- Allottee's withdrawal right: 12-month delay trigger (Clause 7.3)
- Payment terms: booking + 5 construction-linked instalments, totalling 95% pre-possession, balance 5% on offer of possession
- Total paid by Allottee as on 30 September 2024: Rs. [Total-Paid-Placeholder]/- (95% of consideration — see ledger at `02-payment-receipts-2022-2025.docx`)

## Chronology

- **15 June 2022** — Agreement for Sale executed (see `01-builder-buyer-agreement-extract-2022-06-15.docx`).
- **15 June 2022 – 30 September 2024** — Allottee makes all construction-linked instalments on time.
- **28 December 2024** — Three days before promised possession, Promoter issues a delay-acknowledgement letter (`03-builder-delay-acknowledgement-2024-12-28.docx`) re-scheduling possession to [New-Promised-Date-Placeholder].
- **[New-Promised-Date-Placeholder]** — Revised date lapses. No further communication from Promoter. No offer of possession.
- **20 March 2026** — Complainant issues statutory legal notice (`04-statutory-notice-2026-03-20.docx`).
- **20 April 2026** — 30-day compliance window expires. Promoter has not complied.
- **As on filing** — Complainant approaches the District Consumer Commission at [District-Commission-Location-Placeholder].

## Reliefs sought

1. Direction to the Opposite Party to offer immediate physical possession of the apartment together with the occupancy certificate.
2. In the alternative, refund of the entire sum of Rs. [Total-Paid-Placeholder]/- paid by the Complainant with interest at the rate prescribed under the applicable RERA from the respective dates of payment till refund.
3. Compensation of Rs. [Compensation-Sought-Placeholder]/- for mental agony, financial loss, and rental expenditure of Rs. [Rental-Loss-Placeholder]/- incurred during the period of delay.
4. Cost of the notice and litigation: Rs. [Notice-Cost-Placeholder]/-.
5. Any other relief the Commission may deem fit.

## Forum and case type

- **Forum:** District Consumer Disputes Redressal Commission at [District-Commission-Location-Placeholder].
- **Case type:** `district-commission-complaint-section-35`.
- **Statutory anchor:** Section 35 read with Section 34 CPA 2019 (pecuniary < Rs. 50 lakh).
- **Limitation:** Section 69 CPA 2019 — 2 years from date of cause of action. Cause of action arose latest on the lapse of the revised possession date; well within limitation.

## Ingredient check (Verifier-stage)

- ✅ "Consumer" — Section 2(7) CPA 2019 — Allottee purchased apartment for own residence; not for resale.
- ✅ "Deficiency in service" — Section 2(11) CPA 2019 — failure to offer possession on agreed date is per se deficiency (per the line of NCDRC and SC decisions in Pioneer Urban v. Govindan (2019) 5 SCC 725 and Wg. Cdr. Arifur Rahman v. DLF Southern Homes (2020) 16 SCC 512).
- ✅ Pecuniary jurisdiction — under Rs. 50 lakh — District Commission has jurisdiction.
- ✅ Territorial jurisdiction — place of project / place where Complainant resides / place where cause of action arose.
- ✅ Statutory notice not mandatory under CPA 2019 but issued as a matter of good practice.
- ✅ Limitation — within 2 years.

## How to use this fixture

1. Point `read_case_folder(path)` at this directory.
2. Reader extracts facts from the 4 `.docx` files plus this `case-facts-background.md`.
3. Call `get_case_type_format("district-commission-complaint-section-35")`.
4. The remaining 5 agents (Format → Drafter → Verifier → Refiner → Overseer) run end-to-end to produce `final-draft.docx` containing the complaint with Cause Title, Parties, Facts, Cause of Action, Deficiency in Service, Reliefs, Verification, List of Documents, Affidavit.
