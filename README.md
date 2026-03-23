# CVT Authority

**AI-powered CVT transmission repair, acquisition, resale & lease-to-own.**

A complete business playbook for launching and running a CVT-specialized auto repair and BHPH dealership. Built with a 3-agent review pipeline (Devil's Advocate → QA → Final Assembly) to stress-test every assumption.

> **Live Site:** [believable-cat-production-2cf3.up.railway.app](https://believable-cat-production-2cf3.up.railway.app)

---

## What's Inside

### Final Master Action Plan — 11 Sections

| # | Section | What It Covers |
|---|---------|---------------|
| 01 | **Vehicle Scope** | Tier 1 Jatco (Nissan, Jeep, Dodge, Mitsubishi) · Tier 2 Subaru + Honda · Tier 3 Toyota · NHTSA data · 13 class actions · Years 2003–2020 |
| 02 | **Parts Suppliers** | Transtar, Sonnax, Rostra, TransGo, Superior · Part numbers · JF011E rebuild: $1,219–$1,762 · Tooling: $16,900 · Startup inventory: $3,800–$5,500 |
| 03 | **Vehicle Acquisition** | 10 sources ranked · Copart, IAAI, OPENLANE, ACV, Facebook, Craigslist · Salvage/BHPH conflict resolved · Landed costs · Title verification (NMVTIS) |
| 04 | **Legal, Contracts & Insurance** | Dealer + finance licenses · 9 contracts · Insurance $9–22K/yr · FTC CARS Rule · Lemon law states · AI marketing compliance · Entity structure |
| 05 | **In-House Financing** | RISC at 9.9% APR · Realistic ROI: 28–41% · Tiered down payments · Collections Day 1–60 · GAP coverage · GPS trackers · Portfolio sale options |
| 06 | **Intake System & Custom Plan** | 40+ DTC codes by unit · 100-point health score · 5-tier go/no-go matrix · Equipment: $8,500–$13,000 · 4-tier warranty · Repair-or-buy decision tree |
| 07 | **Posting System** | 7 free + 4 paid platforms · 3 FB ad campaigns ($900–$1,400/mo) · Retargeting · SEO · Review generation · Email/SMS sequences · Content calendar |
| 08 | **Website Blueprint** | 6 pages · DMS integration (Wayne Reaves/Frazer) · AI diagnostic report mock · Mobile-first · Schema markup · Offer estimation logic |
| 09 | **Dashboard** | 25+ KPIs with formulas · DMS API workarounds · 7 alert triggers · 9-stage Kanban · Airtable+Retool Phase 1.5 · 15-min daily routine |
| 10 | **Startup Budget** | Monthly burn: $16,100 · Lean minimum: $144K · Recommended: $213K · Break-even analysis · 6-month cash flow · Growth funding (SBA, floorplan, LOC) |
| 11 | **Execution Order** | Track A: repair shop (revenue Week 3) · Track B: dealer license · Phase 0–3 with gates · Risk register (7 risks) · Month 3–6 expansion |

### Additional Documents

- **Original Business Plan** — Revenue model, USP, Facebook campaigns, mechanic training, recruiting, 90-day launch phases
- **Master Plan V1 (Archive)** — Pre-review draft for comparing what changed during the 3-agent pipeline

---

## Site Map

```
/                       → Project Hub (homepage)
/master-plan.html       → Final Master Action Plan (primary document)
/business-plan.html     → Original Business Plan (reference)
/master-plan-v1.html    → Master Plan V1 Draft (archive)
/sitemap.html           → Full Sitemap with section index
```

---

## Tech Stack

| Component | Technology |
|-----------|-----------|
| Server | Node.js + Express |
| Frontend | Static HTML/CSS (no framework) |
| Fonts | Bebas Neue, DM Sans, DM Mono (Google Fonts) |
| Hosting | [Railway](https://railway.app) |
| Theme | Dark (#0a0a0a) with orange (#ff5c00) accents |

---

## Run Locally

```bash
git clone https://github.com/jbellsolutions/cvt-authority.git
cd cvt-authority
npm install
npm start
# → http://localhost:3000
```

---

## Project Structure

```
cvt-authority/
├── server.js                  # Express static file server
├── package.json
├── public/
│   ├── index.html             # Project hub homepage
│   ├── master-plan.html       # Final master action plan (82KB, 1391 lines)
│   ├── business-plan.html     # Original business plan (41KB)
│   ├── master-plan-v1.html    # V1 draft archive (80KB)
│   └── sitemap.html           # Full sitemap & section index
├── LICENSE
└── README.md
```

---

## Review Process

Every section of the master plan went through a 3-agent pipeline:

1. **Devil's Advocate** — Attacked every assumption, found missing data, identified contradictions, flagged unrealistic numbers
2. **QA Agent** — Cross-checked sections for consistency, verified all corrections, ensured no gaps remained
3. **Final Assembly** — Integrated all reviewed content into the final document with proper formatting and cross-references

### Key Corrections Made During Review
- Removed Toyota Camry/Matrix/Sienna and Lexus RX from vehicle scope (no CVTs in US market for specified years)
- Revised startup budget from $40K to $144K minimum after accounting for actual monthly burn ($16,100) and tooling ($16,900)
- Corrected financing ROI from 40–71% to 28–41% after modeling realistic 8–25% default rates
- Resolved down payment contradiction ($500–$1,000 ads vs 20% financing math) with tiered structure
- Identified DMS systems (Frazer/Wayne Reaves) have no public APIs — added Airtable+Retool bridge
- Flagged salvage title + BHPH conflict — segregated clean titles for financing, salvage for cash-only

---

## Deployment

Deployed on Railway with automatic builds from the `main` branch.

```bash
# Deploy manually
railway up

# Or push to main — Railway auto-deploys from GitHub
git push origin main
```

### Environment Variables

| Variable | Default | Description |
|----------|---------|-------------|
| `PORT` | `3000` | Server port (Railway sets this automatically) |

---

## License

MIT
