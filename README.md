# SOPS-Workflows

Central repository for Sky Hardware CC t/a IT Corporation's Standard Operating Procedures (SOPs) and Workflow Process documents — covering bookkeeping, finance, operations, and reporting.

This repo exists so that any workflow document can be picked up, referenced, or handed off — whether that's a colleague, a new team member, or a Claude session — without relying on a single person's institutional knowledge.

---

## Purpose

- **Business continuity** across a small accounts/ops team — if a task needs to be picked up by someone else, the process is written down here.
- **Consistency** — the same task is done the same way every time it's performed, regardless of who's doing it.
- **AI-assisted continuation** — these documents are structured so they can be pasted or linked into a Claude conversation to resume in-progress work without re-explaining context from scratch.

---

## Repo structure

```
SOPS-Workflows/
├── README.md
├── session_summary.md          # rolling handoff notes for in-progress work
├── bookkeeping/                # SOP I-01 – I-12 and related finance SOPs
├── workflow-manuals/           # multi-workflow process manuals (e.g. WP series)
├── operations/                 # QBO Operations Manual and ops-facing procedures
├── reports/                    # source data exports (QBO CSVs) used to build/validate a given month's work
└── archive/                    # superseded versions, kept for reference
```

*(Folders will be created as documents are uploaded — this is the target structure to organise into, not a reflection of what's in the repo yet.)*

---

## Naming convention

| Prefix | Type | Example |
|---|---|---|
| `SOP-I-##` | Individual invoice/bookkeeping Standard Operating Procedure | `SOP-I-01_Standard_Customer_Invoicing.docx` |
| `WP-##` | Workflow Process document (multi-step process, one workflow) | `MA-WP-01_Monthly_Management_Accounts_Compilation_Workflow.docx` |
| `OM` | Operations Manual (broad reference manual, multiple procedures) | `QBO_Operations_Manual.docx` |
| — | Source data / reports | `IT_Corporation_Profit_and_Loss_June_2026.csv` |

New documents should follow this pattern so the index below stays easy to maintain. If a document doesn't fit neatly into a category, flag it rather than forcing a prefix — the convention should stay useful, not become a straitjacket.

---

## Document index

> Update this table each time a document is added or revised. Status reflects whether the document is finalised and in active use, or still being drafted/tested against a live month.

| Document | Type | Status | Version | Last Updated |
|---|---|---|---|---|
| `MA-WP-01_Monthly_Management_Accounts_Compilation_Workflow.docx` | Workflow Process | Draft — being tested against June 2026 live build | 1.0 | 09 Jul 2026 |
| `session_summary.md` | Handoff notes | Living document | — | 10 Jul 2026 |
| QBO Operations Manual | Operations Manual | To be uploaded | — | — |
| Bookkeeping SOP package (I-01 – I-12) | SOP set | To be uploaded | — | — |
| Workflow Process Manual (10 core workflows) | Workflow Process | To be uploaded | — | — |
| ITCorp Workflows Overview | Reference/index | To be uploaded | — | — |
| Staff KPI Dashboard build notes | Reference | To be uploaded | — | — |

*(Rows above with "To be uploaded" are placeholders — replace with the actual filename and details once each document is pushed.)*

---

## Working with these documents in Claude

- **Text files (.md, .csv)** — can be linked directly using the raw GitHub URL, e.g. `https://raw.githubusercontent.com/CJatITCorp/SOPS-Workflows/main/session_summary.md`. Claude can fetch these without needing an upload.
- **Word/Excel files (.docx, .xlsx)** — download from GitHub and upload directly into the chat. Claude can't reliably read binary Office files through a raw link.
- **Starting a new session** — paste or link `session_summary.md` first; it carries the current state of whatever's in progress, plus what still needs to happen next.

---

## Access note

This repository is currently **public**. Some files (QBO exports, workbooks with customer/staff financial data) contain information that shouldn't be publicly visible. Worth confirming this is intentional — if not, switch the repo to **private** under Settings → General → Danger Zone → Change visibility. Private repos still work fine for text files pasted directly into chat; Claude just won't be able to fetch raw links from a private repo without authentication.

---

## Maintainer

Candice Jacobs — Services Operations Coordinator, ITCorp

