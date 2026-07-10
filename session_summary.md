# Session Handoff — June 2026 Management Accounts Build

**Purpose of this doc:** paste this into a new chat to resume exactly where we left off, without re-explaining everything.

---

## Where things stand

1. Built **MA-WP-01: Monthly Management Accounts Compilation Workflow** — a Word doc mapping all 16 tabs of the `IT_Corporation_[Month]_[Year]_Management_Accounts.xlsx` workbook (source: May 2026 file). Covers purpose, QBO data source, manual steps, formula notes, and pitfalls for every tab, plus a QC checklist and file-naming convention.
   - File: `MA-WP-01_Monthly_Management_Accounts_Compilation_Workflow.docx`
2. Started the **live June 2026 build**, working the process for real for the first time.
3. Agreed the list of 13 QBO reports needed to compile June (see below).

## Reports received so far

| Report | File | Status |
|---|---|---|
| P&L, June 2026 (standard) | `IT_Corporation_Profit_and_Loss.csv` | ✅ Usable |
| P&L, June 2025 (standard) | `IT_Corporation_Profit_and_Loss__1_.csv` | ✅ Usable |
| P&L, Mar–Jun 2026 (YTD) | `IT_Corporation_Profit_and_Loss__2_.csv` | ✅ Usable |
| P&L, Mar–Jun 2025 (YTD) | `IT_Corporation_Profit_and_Loss__3_.csv` | ✅ Usable |
| P&L by Class, Mar–Jun 2025 (YTD) | `IT_Corporation_Profit_and_Loss__4_.csv` | ⚠️ Wrong date range — need **June 2025 only**, not YTD (March–May already in workbook from prior months; using YTD would double-count) |
| P&L by Class, Mar–Jun 2026 (YTD) | `IT_Corporation_Profit_and_Loss__5_.csv` | ⚠️ Wrong date range — need **June 2026 only**, same reason |

## Reports still needed

| # | Report | Date | Feeds Tab |
|---|---|---|---|
| 1 | P&L by Class | **1–30 June 2026** | Labour Income Analysis / P&L by Category |
| 2 | P&L by Class | **1–30 June 2025** | Labour Income Analysis / P&L by Category (PY) |
| 3 | Sales by Customer Summary | 1–30 June 2026 | Sales by Customer |
| 4 | Sales by Customer Summary | 1–30 June 2025 | Sales by Customer (PY) |
| 5 | A/R Ageing Summary | as at 30 June 2026 | Customers |
| 6 | A/P Ageing Summary | as at 30 June 2026 | Suppliers |
| 7 | Inventory Valuation Summary | as at 30 June 2026 | Stock valuation |
| 8 | Estimates | 1–30 June 2026, all statuses | Pipeline Report |
| 9 | Balance Sheet | as at 30 June 2026 | Balance Sheet + Cash Movement |

Also needed outside QBO:
- Physical/actual stock count (for Stock valuation tab)
- VAT liability + provisional tax figures (VAT Centre / VAT201) for the Summary tab
- Actual bank/Netcash/Sage Pay/Marketlink closing balances (for Cash Movement, cross-checked against the Balance Sheet)

## Next step when resuming

Re-pull the two by-class reports for June-only (both years), plus items 3–9 above. Once all 13 reports + the non-QBO figures are in hand, work through the workbook in this order (per MA-WP-01, Section 5):

Cover Page → Company Information → P&L - YTD Monthly (CY Only) → P&L vs PY (Month Only) → Labour Income Analysis → P&L vs PY (YTD Monthly) → Profit and Loss by Category → Sales by Customer → Customers → Suppliers → Stock valuation → Pipeline Report → Cash Movement → Balance Sheet → Key Performance Statistics (auto) → Summary (written last) → QC checklist → save/distribute.
