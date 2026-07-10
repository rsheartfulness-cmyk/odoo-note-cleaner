# Kasera Lead Report Cleaner

Browser-only tool for converting raw Odoo CRM lead export files into the approved Kasera follow-up report format.

## How to Use

1. Open `index.html` in a browser, or host this folder on GitHub Pages.
2. Upload the raw Odoo CRM lead export `.xlsx`.
3. Check the dashboard, filters, flags, and preview.
4. Click **Download Report**.
5. Use **Copy Summary** when a short WhatsApp update is needed.

## Hosting

Recommended final URL:

`leadreport.kaseraindustries.in`

This is a static browser app. It does not need a server or database.

Keep these three files together when hosting or sharing the tool:

- `index.html`
- `app.js`
- `excel-lib.js`

## Features

- One row per lead.
- HTML cleanup from follow-up messages.
- Follow-up history merged newest-first.
- Search and filters for stage, salesperson, and flags.
- Stale lead flag, controlled by the stale-days input.
- Hot lead flag for recent high-activity leads.
- Duplicate lead flag.
- Dashboard metrics and top stage/salesperson/tag insights.
- Downloaded workbook includes `Lead Report` and `Summary` sheets.

## Different Export Format

If Odoo column names change, the app first tries automatic matching. If it cannot identify the needed fields, it shows a column-mapping panel.

Required mappings:

- `Opportunity`
- `Message`

Optional mappings:

- `Message Date`
- `Contact Name`
- `City`
- `Salesperson`
- `Stage`
- `Expected Revenue`
- `Tags`

## Privacy

The Excel file is processed inside the user's browser. The lead data is not uploaded or stored anywhere.

## Expected Input

The Odoo export should include these columns:

- `Opportunity`
- `Messages/Contents`

The cleaner also uses these columns when available:

- `Contact Name`
- `Salesperson`
- `Expected Revenue`
- `Stage`
- `Messages/Date`
- `Messages/Created on`
- `Tags/Tag Name`
