# reports/

Status reports. The **top level stays clean** — only two files:
- `README.md` (this file)
- `_report-template.html` — the reusable view skeleton (machinery; leading `_`). Edit it once to restyle every future report.

**Generated reports live in `published/`**, two files per report from the same source:
- `published/YYYY-MM-DD-status.md` — the canonical report (source of truth).
- `published/YYYY-MM-DD-status.html` — a self-contained styled view: double-click to open, share as a single file. Generated from `_report-template.html`. **Never hand-edit it** — regenerate from the `.md` if anything changes.

Keeping generated reports in `published/` leaves the top level uncluttered as reports accumulate over the project — and gives viewers one clean folder to browse.

A report is a **view** — it holds nothing that isn't already in the tracker. Items with **2+ slips** appear at the top under "needs attention."
