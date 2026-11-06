# Client Onboarding & Step-by-Step Notification Delivery Guide

This operational guide provides the exact standard procedure for onboarding a new client business into WingerX Marketing, configuring client contact details (WhatsApp and Email) in the **Notifications** tab, and systematically delivering initial onboarding messages (`MSG_01` to `MSG_05`) via the **Manual Send** tab.

---

## 1. Overview of the Onboarding Workflow

When a new client signs up for Google Business Profile (GBP) marketing management, the account manager must execute a 5-step sequence:

```
[ Step 1: Business Profile Setup ] 
         │ (Connect via Google OAuth or Google Places Search)
         ▼
[ Step 2: Business Context & Brand Identity ]
         │ (Hours, phone, categories, services, brand voice & colors)
         ▼
[ Step 3: Run Initial GBP Health Audit ]
         │ (Auto-analyzes profile completeness, reviews, photos, ranking)
         ▼
[ Step 4: Configure Notifications Tab ]
         │ (Enter client WhatsApp number & Email address, verify opt-in)
         ▼
[ Step 5: Deliver Onboarding Messages (MSG_01 to MSG_05) ]
         │ (Send via Manual Send tab at defined milestones)
         ▼
[ Client Successfully Welcomed & Enrolled in 90-Day Roadmap ]
```

---

## 2. Step 1: Onboarding the Business Profile

You can onboard a new location using either the **Onboarding Wizard** (`/marketing?setup=1`) or from the sidebar under **GBP Integrations**.

### Option A: Via the Onboarding Wizard (`/marketing?setup=1`)
1. In the top-right workspace switcher, make sure you are in **Your workspace** (marked with the `"Your workspace"` badge and user icon).
2. Follow the 4-step wizard:
   * **Step 1 (Connect Google or Search Places):**
     * If the client granted Google Account Manager access, click **Connect Google Account** and authenticate via OAuth.
     * If managing without direct API access, select **Search Google Places**, enter the client's business name and city, and select the location.
   * **Step 2 (Business Context):**
     * Review the business name, address, phone number, website URL, and primary business category.
   * **Step 3 (Syncing):**
     * The system ingests existing business data, reviews, and initial profile score.
   * **Step 4 (Completion):**
     * Click **Go to Marketing Dashboard**.

### Option B: Via GBP Integrations Tab
1. Select **GBP Integrations** in the left sidebar.
2. Click **Add New Location**.
3. Choose **Connect Google Account** or **Add via Google Places**.
4. Confirm details to create the location record.

---

## 3. Step 2: Complete Business Context & Brand Identity

Before sending messages or generating content, ensure the business details are complete:

1. **Location Settings (under GBP Integrations):**
   * **Phone Number:** Verify international E.164 format (e.g., `+919876543210`).
   * **Website URL:** Include `https://`.
   * **Categories:** Set 1 Primary Category and at least 2–3 Secondary Categories.
   * **Services & Attributes:** Add all offered services (e.g., "Emergency Service", "Online Consultations").
   * **Hours:** Set regular operating hours and special/holiday hours.
2. **Brand Identity Tab:**
   * Enter **Brand Voice & Tone** (e.g., "Professional, Empathetic, Authority").
   * Enter **Primary & Accent Colors**.
   * Specify **Prohibited Claims** (e.g., "Never guarantee 100% cure", "No pricing mentions without approval").

---

## 4. Step 3: Run the Initial GBP Health Audit

Running an audit generates the baseline health score and triggers auto-seeding of the **90-Day Growth Roadmap**:

1. Navigate to **GBP Integrations** (or **Location Audits**).
2. Click the **Run Audit** button.
3. Wait 10–20 seconds while the system checks:
   * Profile completeness (Phone, Website, Categories, Hours, Services)
   * Photo count and upload cadence
   * Review volume, average rating, and unreplied reviews
   * Google Q&A presence and special attributes
4. Once completed, note the **Overall Health Score** (e.g., `58/100`), **Critical Issues**, and **Growth Opportunities**.

---

## 5. Step 4: Configure Client Contact Details in the Notifications Tab

To ensure the client receives automated updates and manual messages, configure their WhatsApp and Email channels:

1. In the left sidebar, click **Notifications** (shield icon).
2. Select your client's location from the top location dropdown.

### A. WhatsApp Channel Configuration
1. Click the **WhatsApp Notifications** top tab, then select the **Settings & Preferences** sub-tab.
2. Ensure the **Enable WhatsApp Notifications** toggle is switched **ON**.
3. Fill in:
   * **Client Contact Name:** e.g., `Rajesh Kumar` (used in template variable `{{first_name}}`).
   * **Client WhatsApp Number:** Full international format including country code without spaces or dashes (e.g., `+919876543210` or `+14155552671`).
   * **Timezone:** Select the client's local timezone (e.g., `Asia/Kolkata` or `America/New_York`).
4. **Message Type Subscriptions:** Ensure all message types (`MSG_01` through `MSG_14`) are checked/enabled.
5. Click **Save Settings**.
6. *(Recommended)* Click **Send Test Message** or enter an OTP to verify connection.

> [!IMPORTANT]
> **Meta WhatsApp 24-Hour Customer Window Rule:**
> Meta requires user engagement to open the 24-hour free-form messaging window. To guarantee 100% delivery of marketing templates:
> - Ask the client to send a quick WhatsApp message to your business number (e.g., clicking `https://wa.me/<YOUR_NUMBER>?text=Hi%20WingerX`), OR
> - Send the initial utility icebreaker template with the "Confirm Connection" quick-reply button.

### B. Email Channel Configuration
1. Click the **Email Notifications** top tab, then select the **Settings & Preferences** sub-tab.
2. Ensure the **Enable Email Notifications** toggle is switched **ON**.
3. Fill in:
   * **Client Email Address:** e.g., `client@businessdomain.com`.
   * **Client Name:** e.g., `Rajesh Kumar`.
   * **Timezone:** Select client timezone.
4. Verify all email types (`EMAIL_01` through `EMAIL_14`) are enabled.
5. Click **Save Settings**.

---

## 6. Step 5: Deliver Initial Onboarding Messages (MSG_01 to MSG_05)

Navigate to **Notifications** → **Manual Send** tab. The system provides pre-configured templates categorized under **Onboarding**. Follow this exact sequence over the first 24–48 hours:

```
Timeline:
Day 1 (Hour 0)   ──► MSG_01 (Welcome / Business Connected)
Day 1 (Hour 2)   ──► MSG_02 (GBP Analysis Started)
Day 1 (Hour 4)   ──► MSG_03 (Initial Audit Report Ready)
Day 2 (Morning)  ──► MSG_04 (What We Will Work On — Top Opportunities)
Day 2 (Afternoon)──► MSG_05 (90-Day Growth Roadmap Created)
```

---

### Message 1: MSG_01 — Welcome / Business Connected

* **When to send:** Immediately after onboarding the location and saving phone/email in Notifications.
* **Category:** Onboarding
* **Purpose:** Confirms receipt of details and establishes professional communication.

#### How to Send:
1. In **Notifications** → **Manual Send**, find **MSG_01 — Welcome / Business Connected**.
2. Click **View & Send**.
3. Review the preview variables:
   * `{{first_name}}`: Client's name (auto-filled from settings)
   * `{{brand_name}}`: Your agency or platform name (e.g., "WingerX")
   * `{{business_name}}`: Client's business name
   * `{{business_location}}`: City / Address
4. Click **Send WhatsApp Message** (and/or switch to Email tab and click **Send Email**).
5. **Success Indicator:** Status changes to green `Sent` with timestamp.

#### Message Content:
```text
Hi {{first_name}} 👋

Welcome to {{brand_name}}!

We’ve successfully received your business details for:

📍 {{business_name}}
{{business_location}}

Our team has started analyzing your Google Business Profile.

We’ll review your profile, visibility, reviews, customer activity, profile completeness, and growth opportunities.

Once the analysis is complete, we’ll prepare your personalized report and 90-day growth roadmap.

We’ll keep you updated here.
```

---

### Message 2: MSG_02 — GBP Analysis Started

* **When to send:** 1–2 hours after MSG_01, once you initiate the audit or begin reviewing their listing.
* **Category:** Onboarding
* **Purpose:** Builds transparency and demonstrates active team engagement.

#### How to Send:
1. In **Manual Send**, locate **MSG_02 — GBP Analysis Started**.
2. Click **View & Send**.
3. Verify `{{first_name}}` and `{{business_name}}`.
4. Click **Send WhatsApp Message**.

#### Message Content:
```text
Hi {{first_name}},

We’re currently analyzing {{business_name}} 🔍

Our team is checking:

✅ Google Business Profile completeness
✅ Reviews & reputation
✅ Customer activity
✅ Profile visibility
✅ Business information
✅ Missing opportunities
✅ Areas requiring improvement

Once completed, we’ll share your Business Growth Report and the actions our team will work on over the next 90 days.
```

---

### Message 3: MSG_03 — Initial Report Ready

* **When to send:** Immediately after the initial audit finishes and the Monthly Report / Health Score is generated.
* **Category:** Onboarding
* **Purpose:** Delivers high-value tangible insights with their overall growth score.

#### How to Send:
1. In **Manual Send**, locate **MSG_03 — Initial Report Ready**.
2. Click **View & Send**.
3. Confirm variables:
   * `{{overall_score}}`: Calculated audit score (e.g., `64`)
   * `{{critical_issue_count}}`: Number of high-priority audit findings (e.g., `3`)
   * `{{improvement_count}}`: Number of medium opportunities (e.g., `5`)
   * `{{strength_count}}`: Number of passing checks (e.g., `8`)
   * `{{report_link}}`: Direct URL to client-facing report or dashboard
4. Click **Send WhatsApp Message**.

#### Message Content:
```text
Great news, {{first_name}} 🎉

Your analysis for {{business_name}} is complete.

📊 Business Growth Score: {{overall_score}}/100

We identified:
🔴 {{critical_issue_count}} important issues
🟡 {{improvement_count}} growth opportunities
🟢 {{strength_count}} areas performing well

Our team has also created a prioritized action plan for your business.

👉 View your complete report:
{{report_link}}
```

---

### Message 4: MSG_04 — What We’ll Work On

* **When to send:** Next morning (Day 2), before launching Phase 1 tasks.
* **Category:** Onboarding
* **Purpose:** Summarizes the top 4 immediate focus areas so the client understands the immediate value.

#### How to Send:
1. In **Manual Send**, locate **MSG_04 — What We Work On**.
2. Click **View & Send**.
3. Ensure the top 4 findings are populated:
   * `{{finding_1}}`: e.g., "Add missing business phone & primary category"
   * `{{finding_2}}`: e.g., "Respond to 6 unreplied customer reviews"
   * `{{finding_3}}`: e.g., "Upload 10 high-resolution interior & exterior photos"
   * `{{finding_4}}`: e.g., "Create weekly Google update posts targeting local keywords"
   * `{{roadmap_link}}`: Link to the 90-Day Roadmap tab
4. Click **Send WhatsApp Message**.

#### Message Content:
```text
Hi {{first_name}},

Based on our analysis of {{business_name}}, these are the main areas our team will focus on:

1️⃣ {{finding_1}}
2️⃣ {{finding_2}}
3️⃣ {{finding_3}}
4️⃣ {{finding_4}}

We’ll work through these based on priority and keep you updated as improvements are completed.

👉 View your complete plan:
{{roadmap_link}}
```

---

### Message 5: MSG_05 — 90-Day Growth Roadmap Created

* **When to send:** Afternoon of Day 2, once Phase 1 tasks are confirmed in the **Tasks** tab.
* **Category:** Onboarding
* **Purpose:** Sets long-term expectations for the 3-month growth trajectory (Foundation → Visibility → Performance).

#### How to Send:
1. In **Manual Send**, locate **MSG_05 — 90-Day Roadmap Created**.
2. Click **View & Send**.
3. Verify `{{business_name}}` and `{{roadmap_link}}`.
4. Click **Send WhatsApp Message**.

#### Message Content:
```text
We’ve created a personalized 90-day growth roadmap for {{business_name}} 🚀

📅 Month 1 — Fix & Optimize
Our team will focus on correcting profile issues, improving business information, categories, services, hours, profile content, and other important setup areas.

📅 Month 2 — Visibility & Reputation
We’ll focus on reviews, customer engagement, profile activity, fresh content, media, and improving your overall Google presence.

📅 Month 3 — Growth & Performance
We’ll analyze performance and focus on increasing valuable customer actions such as calls, website visits, directions, bookings, and enquiries.

👉 View your complete roadmap:
{{roadmap_link}}
```

---

## 7. Verifying Delivery & Troubleshooting

1. **Message History Tab:**
   * After sending, switch to the **Message History** tab under Notifications.
   * Verify the record displays:
     * **Message Type:** e.g., `MSG_01`
     * **Recipient:** Client phone number
     * **Status:** `SENT` (green) or `DELIVERED`
     * **Sent At:** Timestamp
2. **If Status Shows `FAILED`:**
   * **Phone format error:** Verify number starts with `+` and country code (e.g., `+91`, `+1`).
   * **Meta window expired:** Send the Utility Icebreaker (`EMAIL_00` or `wingerx_utility_campaign_00`) with quick-reply button.
   * **Email fallback:** Immediately send the corresponding email (`EMAIL_01` through `EMAIL_05`) via **Email Notifications** → **Manual Send**.
3. **Resending a Message:**
   * You can resend any message at any time by clicking **View & Resend** in the Manual Send list.
