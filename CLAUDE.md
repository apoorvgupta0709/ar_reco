# CLAUDE.md — A & R Financial Reconciliation

## What this folder is

This is **not a software project.** It is a personal **matrimonial financial reconciliation** between:

- **A = Apoorv** — the user (it@itarang.com). Salaried at Tata Steel.
- **R = Rupinder** (also "Roop") — his wife.

R shared a spreadsheet claiming a large net contribution gap in her favour. A is building an evidence-based counter-analysis from raw bank statements, credit-card extracts, and salary slips to test, correct, and rebut that claim, and to draft a reply.

> **Sensitive personal & potentially legal material.** Treat all figures, account numbers, and family details as confidential. Nothing here is legal or financial advice — the numbers are inputs to a lawyer's/CA's view, not a settlement figure.

## Current bottom line

| Position | Gap (R − A) | Source |
|---|---:|---|
| R's latest claim (27 Jun file) | **₹40,06,672** in R's favour | `Emails/Rupinder 27062026 file.xlsx` → `Top sheet` J14 |
| R's earlier claim (16 May file) | ₹35,62,672 in R's favour | her May file's Top sheet J14 (file not in repo; verified in `Cross-check findings.md`) |
| A's rebuttal to the **27-Jun** file (cashflow, validated data) | **~₹10.08L in A's favour** on her till-Aug basis; **₹7.81L** after concessions; ₹11.96L on the May basis — quote the band **₹8–12L in A's favour** (pending R's statements) | `Rebuttal v2 findings.md` §1.2 |

> **The ₹5.49L copy error (found 7-Jul-2026):** R's 27-Jun Top sheet row 18 starts from "old sheet R−A = ₹30,13,962" — but her old gap was ₹35,62,672; the ₹30,13,962 is **A's Common-Household B1 figure copied from A's 26-May reply file** (exact to the rupee). On her own method her FINAL is **+₹32,09,224, not +₹37,57,934**. The real May→June top-sheet movement is +₹4,44,000: EMI extension +₹1.47L (partly *projected* Jul/Aug 2026 payments), an unexplained ₹2.56L cut to A's rent credit (disputed — Axis shows ₹4,21,202 of A-paid 2024 rent that her new table zeroes), Tiago −₹0.66L, maid/school +₹1.07L. See `Rebuttal v2 findings.md` §1.1.

> **R's 27-Jun move:** she added a new **₹37.34L "Rest of the expenses" sheet** (day-to-day spend) → FINAL claim R−A = +₹37,57,934 (**₹32.09L** once the copy error is corrected). A's stance (per `Rebuttal v2 findings.md`): that sheet is **unvalidated** (no statements) and **double-counts itself** (a ₹9.56L "Splitwise household" lump layered over itemized rows, mostly 2018–19), so it does not enter the reco. On the **same basis A's own documented day-to-day + personal spend is ~₹47L** (larger than her ₹37.34L) → the day-to-day is symmetric, not owed by A. So cashflow sits at **~₹10.08L in A's favour** (till-Aug basis, rent cut restored; ₹7.81L after the ₹2.27L concessions) pending R's statements. The real substance is now: the **four-asset reconciliation** (One DXP/Sobha/Tiago/XUV — A's side stress-tested to source: **₹43.24L hard-verified** of ₹51.14L claimed; the ₹7.9L gap = property TDS ₹2.74L + both car payments ₹5.16L, paid from the still-pending HDFC/ICICI accounts. One DXP down ₹14.5L + both EMI streams tie exactly; Sobha corrected to ₹11.06L after removing a ₹1.25L CC double-count; A owed ~₹10–11L on Sobha; R's ₹21L XUV reduced by the Oorvi ₹9.91L), the **Oorvi finding**, and **A's income statement** (₹1.71Cr net fully consumed, ~zero liquid savings — Noida-house-yet-shifted-to-Gurgaon lifestyle).

A's rebuttal additionally flags **asset-equity claims handled separately** (not in the cashflow gap): Sobha EMI share ~₹6.28L, refundable security deposit ₹2.6L, marital-era investments ₹46.99L.

These numbers **evolve as more statements arrive** (HDFC/ICICI savings still pending at last update). Always re-confirm the headline figure against the latest workbook before quoting it.

## Conventions

- **"Gap" = R − A.** Positive = R contributed more (R's framing); A's analysis drives it negative.
- Currency is **INR**, written in **lakh (L) / crore** notation (₹1L = 100,000; ₹1Cr = 100L).
- People: `A` / `Apoorv`; `R` / `Rupinder` / `Roop`; `Oorvi` = their daughter.
- **Canonical output:** `Reco Files/Apoorv_Master_Reconciliation_FINAL.xlsx` is the single source of truth. `Other Draft/` holds **superseded** versions — read-only history; do not edit or cite as current.

## File map

### Primary workbooks
- **R's file (her claim, current):** `Emails/Rupinder 27062026 file.xlsx`
  Sheets: `Top sheet`, `Rest of the expenses by R`, ` EMI till May`, `Rent& utilities`, `Maid salaries`, `Oorvi's school`, `EMI acc txn dump`. Headline: R − A = ₹40,06,672 (`Top sheet` J14; A total I13 ₹89.92L, R total J13 ₹1,29,98,468). Supersedes the earlier `…June 26.xlsx` version.
- **A's rebuttal (current):** `Reco Files/Apoorv_Master_Reconciliation_FINAL.xlsx`
  Sheets: `0. Swing Summary`, `1. Wrong Claims + Diffs + Reorg`, `2. Monthwise Breakup`, `3. All Expenses Rowwise`, `4. Category Summary`, `5. BoB EMI Detail`, `6. TEHP & Income`, `7. Common Household Detail`. Workbook headline: −₹11,96,028 (May basis; see "Current bottom line" above for the till-Aug band).

### Email exchange (`Emails/`)
The back-and-forth, as PDF, plus R's latest workbook:
- `Rupinder 16052026.pdf` — R's email (16 May 2026).
- `Apoorv 26052026.pdf` — A's reply (26 May 2026).
- `Rupinder 27062026.pdf` + `Rupinder 27062026 file.xlsx` — R's latest email and revised claim (27 Jun 2026).

### Analysis write-ups (root, markdown)
- `Master summary.md` — the master cross-check; tier-by-tier walk from ₹35.6L claim down. Most complete narrative.
- `Cross-check findings.md` — arithmetic verification of R's file + structural/framing critique.
- `Credit card findings.md` — ICICI + HDFC credit-card analysis (Sobha CC payment, jewellery, childbirth).
- `Reply to Rupinder 27062026.md` — **the current outward-facing reply** (email body + Annex A–F): the ₹5.49L copy error, both sides of the seven heads, the ₹47.59L additions walk, the Oorvi ledger, and the day-to-day symmetry table. (The superseded May-round draft `Email reply to R.md` was deleted 9-Jul-2026; its A/B/C structure lives on in `Emails/Apoorv 26052026 file.xlsx` and git history.)
- `Rebuttal v2 findings.md` — the internal analysis record behind that reply: her arithmetic restated with the copy error (§1), the who-paid teardown of her ₹37.34L "Rest of expenses" (§2), the Oorvi net-flow analysis (§3), the four-asset reconciliation (§4), and income-vs-deployment (§5).

### Evidence (`Bank Statements/Accounts/`)
- **Axis personal** `915010015602288` — `axis statement/` (2018–2026), `AXIS FY23-25 Oct.xlsx`.
- **BoB joint a/c** `78770100030383` — `bob/`, `bob 2/`, `CY23/CY24 Bob.xlsx`, `BoB_Joint_Account_Analysis.xlsx`.
- **HDFC / ICICI savings** — `hdfc/`, `15102025/` (loan/ledger reports).
- **Credit cards** — `amazon cc/` (ICICI Amazon Pay ×8006 PDFs), `HDFC CC/` (Tata Neu ×46 PDFs).
- **Oorvi's account** — `Oorvi/` (2022–2026 PDFs).
- **Salary slips** — `salary slip/` (~113 Tata Steel slips, UUID-named + year PDFs).
- **Derived:** `Apoorv_Axis_Reconciliation_3yr.xlsx`, `BoB_Joint_Account_Analysis.xlsx`.
- `cc_all_transactions.csv` (root) — 771 categorized CC transactions. Columns: `card, card_last, stmt_date, date, sno, description, amount, is_credit, source, category, subcategory`.

## Glossary of entities

- **One DXP** — main property; joint home loan (a/c `78770600001599`, disbursed ₹1,75,21,000).
- **Sobha** — second property; loan (a/c `73960600003596`, disbursed ₹77,55,997) **transferred to R** → now R's solo asset. A funded Sobha down-payment + ₹3.75L direct (Axis ₹2.5L + CC ₹1.25L on 05-Feb-2024) + ~₹6.28L EMI share.
- **Car Tiago** — loan **transferred to A** → now A's asset; R contributed ₹6.58L.
- **Car XUV 700** — A ₹4.5L, R ₹21L.
- **BoB `78770100030383`** — joint account; both loans' EMIs run through it. A funded ~55.2% of identified inflows, R ~44.8%.
- **Oorvi account `922010006635569`** — Axis minor account, **"OORVI GUPTA U/G APOORV GUPTA"** (A is guardian). Funded mostly by ₹10.14L grandparent gifts; net **₹9.91L flowed out to Rupinder** (vs ₹0.78L in). Central to rebutting R's "A borrowed Oorvi's money" claim — see `Rebuttal v2 findings.md` §3.
- **TEHP** — Tata Steel family-holiday perquisite; A claims true after-tax cost (~₹3.65L).
- **NRI rent TDS** — ₹16,536/month TDS on rent to an NRI landlord (from Dec 2024); reclassified from property-TDS to rent.

## How to work with the data

- **Read `.xlsx`** with `python3` + `openpyxl` (`load_workbook(path, read_only=True)`; use `data_only=True` for computed values). Legacy **`.xls`** files need `pandas`/`xlrd`.
- **CC PDFs are already extracted** into `cc_all_transactions.csv` — prefer the CSV over re-parsing PDFs.
- **Tie every total back to a source statement.** The four markdown docs document where each figure ties (e.g. Axis outflow ₹1.15Cr, BoB inflows, CC buckets). When recomputing, reconcile to those.
- **Do not edit `Other Draft/`** — it's superseded. Make `FINAL.xlsx` the only live workbook; if producing a new version, supersede cleanly and note it here.

## Framing caveats (important)

This is an **expense-only cashflow reconciliation.** It deliberately excludes, and must not be confused with, a full settlement: **asset distribution** (properties, vehicles, jewellery, investments, EPF/PPF/NPS), **income disparity** (A's ~₹2.19Cr gross / ₹1.71Cr net over FY19–FY26), and **maintenance / child custody**. A ₹0 expense gap is not a ₹0 settlement, and a ₹35L expense gap is not a ₹35L settlement. Keep the cashflow number and the asset-equity claims clearly separated, exactly as `Reply to Rupinder 27062026.md` Annex F does.
