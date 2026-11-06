# Monthly Report Feature Guide

The **Monthly Report** tab aggregates and synthesizes all marketing performance, content output, customer review sentiment, search discovery metrics, and audit findings into an executive-ready monthly report for any selected month (`YYYY-MM`).

> **Navigation:** Go to https://app.wingerx.com/marketing page and click the **Monthly Report** tab.

---

## 1. Prerequisites
- A location must be selected.
- At least one audit, post, or review should exist in the target month for complete reporting.

---

## 2. Key Components & How to Use Them

### A. Period Selector & Report Generation
* **Reporting Period:** Standardized `YYYY-MM` picker (e.g., `2026-10`, `2026-11`).
* **"Generate / Refresh Report" Button:**
  * When clicked, calls `POST /locations/{id}/monthly-reports` to re-aggregate live database tables.
  * Ensures all newly published posts, answered reviews, and metric entries are factored in.

---

### B. Executive Summary KPI Cards
Four primary summary cards benchmark monthly health:

| Metric Card | Definition | Healthy Benchmark |
|---|---|:---:|
| **Published GBP Posts** | Total Google update posts published during the period. | 8–12 posts / month |
| **Reviews Answered** | Total customer reviews responded to vs. received. | 100% response rate |
| **Search & Maps Views** | Total Google discovery and direct search impressions. | Growth over prior month |
| **Compliance Score** | Content safety & policy score (percentage with 0 policy flags). | 100% |

---

### C. Customer Discovery & Actions Panel
Breaks down how potential customers interacted with the Google Business Profile:
* **Profile Impressions:** Searches on Desktop vs. Mobile Maps.
* **Website Clicks:** Visitors directed to the client's website.
* **Phone Call Inquiries:** Direct phone calls placed from the listing.
* **Direction Requests:** Driving directions requested to the physical storefront.

---

### D. Content & Review Output Breakdown
* **AI Posts Generated:** Total volume of drafts generated.
* **Posts Approved & Published:** Actual volume approved and posted to Google.
* **Review Sentiment Distribution:** Percentage of 5-star, 4-star, and negative reviews received during the month.
* **Average Response Time:** Speed at which customer reviews were replied to.

---

### E. Keyword Growth & Visibility
* **Active Target Keywords:** Tracked high-intent local search terms.
* **Rank Movement:** Keywords that gained top 3, top 5, or top 10 local pack visibility.

---

### F. Sharing the Report with Clients
1. Copy the public or client-facing link from the top share button.
2. Deliver the summary to the client via the **Notifications** tab → **Manual Send** using `MSG_13` (WhatsApp) and `EMAIL_13` (Email).
