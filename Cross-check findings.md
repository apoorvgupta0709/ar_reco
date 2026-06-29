# Cross-check of "A and R Financials reconciliation.xlsx"

**Date of review:** 21 May 2026
**File reviewed:** `A and R Financials reconciliation.xlsx` (6 sheets: Top sheet, EMI, Rent & utilities, Maid salaries, Oorvi's school, EMI acc txn dump)
**Bottom-line claim in the file:** R's total contributions exceed A's by **₹35,62,671.82** (Top sheet cell J14).

---

## 1. What the file is doing

The Top sheet aggregates contributions by category, splits each category into Down Payment / TDS / EMIs, and then sums per person:

| Category | A total | R total |
|---|---:|---:|
| One DXP (property) | 54,66,704.18 | 53,08,994 |
| Sobha (property — loan transferred to R) | 3,52,092 | 7,03,250 |
| Car Tiago (loan transferred to A) | 0 | 6,58,224 |
| Car XUV 700 | 4,50,000 | 21,00,000 |
| Rent | 25,53,000 | 13,54,000 |
| Maid salaries | 0 | 17,92,000 |
| Oorvi's school | 0 | 4,68,000 |
| **Total** | **88,21,796.18** | **1,23,84,468.00** |
| **R − A** |   | **35,62,671.82** |

---

## 2. Arithmetic verification — what ties out

I recomputed every total from the underlying detail.

- ✅ Top sheet column totals (I13, J13) and the R − A figure (J14) **add up correctly** given the per-row totals.
- ✅ Rent & utilities tab sums (25,53,000 A and 13,54,000 R) match Top sheet.
- ✅ Maid salaries tab sums (0 A and 17,92,000 R) match Top sheet.
- ✅ Oorvi's school tab sum (4,68,000 R) matches Top sheet; 28 monthly entries Feb 2024 – May 2026.
- ✅ Sobha down payment (3,52,092 A and 7,03,250 R) is internally consistent.
- ✅ Car Tiago and Car XUV 700 row totals are arithmetically consistent.
- ✅ Loan disbursement totals on the bank dump match Top sheet:
   - 78770600001599 (One DXP loan): **₹1,75,21,000** ✓
   - 73960600003596 (Sobha loan): **₹77,55,997.24** ✓
- ✅ Rupinder's EMI sheet column (L) sums to **₹31,04,086** and ties exactly to the bank dump line by line.

---

## 3. Discrepancies I found

### Issue 1 — Apoorv's EMI total is overstated by ₹20,000

- The EMI sheet column C ("APOORV") sums to ₹38,44,967.18 (matches Top sheet G4).
- The bank transaction dump shows only ₹38,24,967.18 of payments narrating APOORV.
- There is **one extra ₹20,000 entry** in the EMI sheet that does not appear in the bank dump (row C30 — `20000`).
- **Effect:** This *overstates* A's contribution by 20,000, which makes the R − A gap (her claim) appear ₹20,000 *smaller* than it would otherwise be. Correcting this would push the gap to ~₹35,82,671.82 — i.e., **it favours her, not you**.

### Issue 2 — One DXP row: R's total is short by ₹65,330 vs. its components

For the One DXP row, R's components are:
- Down payment R (D4): 22,04,908
- TDS R (F4): 65,330
- EMIs R (H4): 31,04,086
- **Sum = 53,74,324**

But the stated Total R (J4) is **53,08,994** — exactly 65,330 less, i.e., the TDS R figure was left out of the row total.

- **Effect:** R's total contribution is *understated* by 65,330. Correcting this would push the gap to ~₹36,28,001.82 — again, **favours her, not you**.

### Issue 3 — The bank dump's stated grand total is off by ₹1,69,000

- The CR column footer (J123) shows **₹3,20,45,127.14**.
- Summing every credit line by line gives **₹3,22,14,127.14** — exactly one Rupinder NEFT (₹1,69,000) more.
- This is a stale total in the dump itself, not a recon error. Doesn't affect the conclusion, but tells you the underlying data hasn't been refreshed cleanly.

### Issue 4 — ₹5,000 credit from "OORVIGUPTAUGAPO" not attributed to either side

- A ₹5,000 transfer on 06/10/2024 narrating `OORVIGUPTAUGAPO` (likely Oorvi's minor account) lands in the loan account but isn't credited to A or R in the EMI sheet.
- Probably immaterial, but worth understanding whose money funded that account.

---

## 4. What is **not** verifiable from this file

The arithmetic ties out, but the **underlying claims about who paid what** are not supported by source documents in this workbook. You'd want statements / payment proofs for:

1. **One DXP down payments**: A 14,50,000 + R 22,04,908. No bank-statement evidence in the file.
2. **Sobha down payments**: A 2,50,000 + R 7,03,250. No evidence.
3. **TDS payments**: A 1,71,737 (One DXP) + 1,02,092 (Sobha) and R 65,330 (One DXP). No 26AS / TDS challan attached.
4. **Car Tiago**: R's EMIs of 5,08,224 are a single figure with no detail or transaction dump.
5. **Car XUV 700**: A 4,50,000 + R 21,00,000 — no invoice or payment proof; no clarity on who is on the registration.
6. **Rent & utilities, maid salaries, school**: only summarised by year; no underlying receipts.

---

## 5. Structural / framing questions to raise before agreeing to ₹35,62,671.82

These are not arithmetic errors — they're choices in the model that materially change the outcome.

**a. The "loan transferred to…" notes change ownership but the file doesn't reconcile the transfer**
- Sobha: loan was transferred to R. A had paid 2,50,000 down + 1,02,092 TDS + (some portion of) EMIs before transfer. Were these reimbursed to A at transfer? If not, why are they still on A's side?
- Car Tiago: loan was transferred to A. R paid 1,50,000 down + 5,08,224 EMIs **on a vehicle now owned by A**. By the same logic that puts those amounts on R's side, A would owe R that 6,58,224 only if A also kept the asset's value. Did A take the car at book value, or with a payout?

**b. The Sobha EMIs are folded into the One DXP EMI totals ("included above")**
- The EMI dump is for a joint account holding *both* One DXP and Sobha loans. The Top sheet treats all EMI payments as One DXP EMI. Until the Sobha-loan transfer date, some portion of A's and R's EMI transfers were servicing the Sobha loan — which is now entirely R's asset. The split between One DXP EMI and Sobha EMI before transfer is not shown.

**c. Equity vs. cashflow — the file equates "who paid" with "who is owed"**
- The model treats every category symmetrically: each rupee one party paid is a rupee owed to them. That works for shared *expenses* (rent, maid, school). It does **not** automatically work for *assets* (down payments, EMIs on properties / cars), because the asset's current value, ownership share, and future EMI obligation all matter. A 50:50 owner who paid 60% of historical EMI isn't necessarily owed 10% — it depends on what each party walks away with.
- The Top sheet hints at this with "Roop future EMI" and "Apoorv future EMI" columns showing the **future** EMIs split 50:50, but the historical EMIs are split ~55:45 (A higher) on One DXP and 0:100 (R) on Tiago. The historical splits are accepted at face value.

**d. Missing categories that may exist on A's side**
- The expense buckets listed (rent, maid, school) are all categories with **zero or near-zero A contribution**. Categories where A may have outsized contribution are absent: groceries, utilities (despite the rent tab being labelled "Rent & utilities", no utility line items appear), travel/vacations, medical, insurance premiums, Oorvi's clothes/activities outside school, household goods, dining, fuel.
- If A funded any of those, none of it is credited here. Whether that's appropriate depends on whatever framework you and R have agreed for the split.

**e. The "Total A" baseline excludes A's larger non-overlapping contributions**
- Standard practice in a separation reco is to list **all** material cash outflows from both sides, even those the other party did not contribute to, then net out. This file only lists the seven categories above. If A's salary went into a joint account that paid for many other things, none of that is here.

**f. Joint vs. personal account flows**
- All EMI transfers in the dump come from accounts ending in `IMPSAXB91783859` (Apoorv) or `AXOMB…RUPINDER SAINI` (Rupinder). If either of those is fed from a *joint* account or from the other person's income, attributing the payment 100% to the named transferor may not be accurate.

---

## 6. Suggested next steps

If you want to push back rigorously, in order of impact:

1. **Get clarity on the loan-transfer mechanics** (issue 5a). The Tiago transfer in particular: 6,58,224 of R's claim depends on whether A took that car with a corresponding settlement.
2. **Pull the Sobha EMI split** out of the One DXP EMI bucket. The "included above" treatment makes it impossible to see how much of each person's EMI was servicing the Sobha (now R's) loan.
3. **Agree on the framework** (issue 5c): are we splitting historical cash, equalising future asset value, or some hybrid? The 35.6L figure is only the answer to the first of those.
4. **Request source backup** for the unverified figures in §4 above (down payments, TDS, car payments, rent/maid/school receipts). The arithmetic is sound, but the inputs aren't proven.
5. **Surface your contributions not captured** in §5d, with bank statements or receipts.
6. **Note the two small arithmetic items** (Issues 1 and 2) for cleanliness — but be aware both currently favour you slightly; correcting them widens the gap by ~₹85,000 in her favour.

---

*This document checks the file's internal arithmetic and identifies structural assumptions. It does not constitute legal or financial advice — please review the framework and any settlement with your lawyer / CA.*
