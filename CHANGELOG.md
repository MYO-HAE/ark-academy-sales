# Ark Academy Sales Pipeline — Nightly Build

**Build Date:** February 25, 2026 (01:00 KST)  
**Status:** ✅ SUCCESS — Live and accessible

---

## What I Built

**Ark Academy Sales Pipeline Dashboard** — A visual CRM for tracking B2B school leads, demos, and pilot program negotiations for Ark Academy's AI literacy curriculum.

### Features

- **Pipeline Overview** — 6 key metrics: Total Leads, Pipeline Value, Active Demos, Pilot Negotiations, Closed Won, Follow-ups Needed
- **Monthly Targets** — Visual progress bars for February goals (schools contacted, demos scheduled, pilot proposals, revenue)
- **Kanban-Style Pipeline** — 4 stages: Initial Contact → Demo Scheduled → Proposal Sent → Pilot/Closed
- **Lead Cards** — School name, type, estimated value, days since contact/urgency indicators
- **Recent Activity Feed** — Chronological log of calls, emails, demos, and wins
- **Quick Actions** — Proposal email templates, demo scheduler, website link
- **Dark Premium UI** — Matching Ark Academy brand with smooth gradients

### Mock Data Included

12 active school leads across international schools and academies in Seoul area:
- Seoul International School (₩30M)
- Dulwich College Seoul (₩35M) — Demo Feb 27
- Chadwick International (₩28M) — Demo Feb 28
- SFS Academy (₩40M) — Proposal sent
- Seocho Academy (₩25M) — **WON**
- Mapo EdTech Consortium (₩35M) — Negotiating

**Total Pipeline:** ₩240M

---

## Why It Helps

From USER.md analysis:
- Ark Academy sales/marketing is flagged as **priority**
- David runs Korea ops and needs visibility into B2B outreach
- No existing CRM/sales tool in the nightly-builds folder
- Previous dashboards focused on tasks, grants, learning — but not sales pipeline

This dashboard gives David a **single view of all school leads** with urgency indicators, estimated values, and next actions.

---

## Live URL

🌐 **https://ark-academy-sales-2026.pages.dev**

✅ Deployed successfully via Cloudflare Pages (HTTP 200 verified)

Preview URL: https://64e7999b.ark-academy-sales-2026.pages.dev

---

## GitHub Repo

📁 **https://github.com/MYO-HAE/ark-academy-sales**

```bash
git clone https://github.com/MYO-HAE/ark-academy-sales.git
cd ark-academy-sales
# Open index.html in browser or serve with any static server
```

---

## How to Test Locally

```bash
cd /Users/davidkim/.openclaw/workspace/nightly-builds/ark-academy-sales
python3 -m http.server 8080
# Open http://localhost:8080
```

Verify:
1. Header loads with "Ark Academy — B2B Sales Pipeline"
2. 6 stat cards display at top
3. February targets show progress bars
4. 4 pipeline columns with lead cards
5. Red "hot" indicators for urgent items (Due Feb 27-28)
6. Recent activity feed with 4 entries
7. Quick action buttons work

---

## Deployment Log

| Step | Status | Notes |
|------|--------|-------|
| Scaffold project | ✅ | Single-file HTML dashboard |
| Build dashboard | ✅ | Full UI with mock data |
| Create wrangler.toml | ✅ | Cloudflare Pages config |
| Git init & commit | ✅ | Initial commit |
| Create GitHub repo | ✅ | MYO-HAE/ark-academy-sales |
| Push to GitHub | ✅ | main branch |
| Deploy to Cloudflare | ✅ | Using wrangler CLI |
| Verify live URL | ✅ | HTTP 200 OK |

---

## Tech Stack

- Single-file HTML/CSS/JS (no build step)
- Vanilla JavaScript (no frameworks)
- Mock data (Notion Leads DB integration ready)
- Mobile-responsive design
- Cloudflare Pages hosting

---

## Next Optimization

1. **Notion Leads DB Integration** — Pull real leads from Ops HQ
2. **Add Lead Form** — Create new leads directly from dashboard
3. **Email Templates** — Pre-written proposal/demo follow-up emails
4. **Calendar Integration** — Show upcoming demos on calendar view
5. **Revenue Forecasting** — Weighted pipeline by probability
6. **School Research** — Auto-populate school info from web search

---

## Files

- `index.html` — Single-file dashboard (22KB, inline CSS/JS)
- `wrangler.toml` — Cloudflare Pages config
- `CHANGELOG.md` — This file

---

**Note:** Dashboard is live and functional. All data is mock/demo data for UI demonstration.

