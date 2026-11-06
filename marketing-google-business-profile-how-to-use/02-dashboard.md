# Dashboard & Onboarding Overview

The **Dashboard** tab serves as the central command cockpit for the selected Google Business Profile location. It provides instant visibility into location health, onboarding progress, live KPI metrics, pending approvals, and recent marketing activity.

> **Navigation:** Go to https://app.wingerx.com/marketing page and click the **Dashboard** tab.

---

## 1. Prerequisites
- A workspace must be selected.
- A location must be selected from the top location dropdown (or onboard a new one if none exists).

---

## 2. Key Components & How to Use Them

### A. Location Header & Health Status
Located at the very top of the dashboard:
* **Business Name & Category:** Displays the official GBP profile name, primary category, and full physical address.
* **Connection Badge:**
  * `Google Connected` (Green): Profile is linked via Google OAuth with direct API access.
  * `Places Managed` (Blue): Profile is tracked via Google Places search for manual workflows.
* **Overall Profile Health Score:** Shows the latest computed audit score (e.g., `78/100`) with color-coded status badge (`Healthy`, `Needs Attention`, `Critical`).

---

### B. Summary Metric Cards
Four real-time performance indicators are displayed across the top row:

| Stat Card | Source Data | What It Measures |
|---|---|---|
| **Monthly Views** | Google Insights / Aggregate Metrics | Total impressions across Google Search and Google Maps for the current 30-day period. |
| **Reviews & Rating** | Google Review Sync | Total reviews count alongside the profile's average star rating (e.g., `4.8 ★ (124 reviews)`). |
| **Active Keywords** | Keywords Database | Count of keywords currently tagged as `ACTIVE` and tracked for local rank movement. |
| **Pending Approvals** | Approval Queue | Count of AI-generated posts, review replies, or edits awaiting human sign-off before publishing. |

---

### C. Onboarding Checklist
For new locations, the Onboarding Checklist guides the operator through critical setup milestones:

```
[✓] Step 1: Connect Business Listing (OAuth or Places)
[✓] Step 2: Complete Business Context (Phone, Address, Hours, Services)
[✓] Step 3: Establish Brand Identity (Voice, Primary Colors, Prohibited Claims)
[ ] Step 4: Run Initial GBP Health Audit
[ ] Step 5: Configure Notifications & Deliver Onboarding Messages (MSG_01 to MSG_05)
[ ] Step 6: Schedule First Month Content (Calendar & Smart Posts)
```

* **Progress Bar:** Reflects completion percentage (e.g., `4/6 Completed - 66%`).
* **Direct Navigation:** Clicking any uncompleted step navigates directly to the corresponding tab.

---

### D. Recent Activity Stream
Displays a live timeline of recent marketing actions performed on this location:
* Automated pipeline executions
* Content approvals and publishing events
* Incoming Google customer reviews
* WhatsApp / Email notification deliveries

---

### E. Quick Action Buttons
At the top right of the dashboard:
* **"Run Audit":** Triggers an immediate GBP health audit (or click the **GBP Integrations** tab).
* **"New Post":** Opens the Smart Post generation modal (or click the **Smart Posts** tab).
* **"View Roadmap":** Jumps directly to the 90-Day Growth Roadmap (or click the **Tasks** tab).
