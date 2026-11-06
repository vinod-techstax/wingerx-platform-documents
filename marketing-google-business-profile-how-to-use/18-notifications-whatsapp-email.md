# Notifications Module (WhatsApp & Email Channels)

The **Notifications** tab manages automated and manual client communication across **WhatsApp** and **Email**. It allows agency account managers to keep business owners informed about audits, task completions, new reviews, and monthly growth reports without leaving the platform.

> **Navigation:** Go to https://app.wingerx.com/marketing page and click the **Notifications** tab.

---

## 1. Prerequisites
- A location must be selected.
- Client phone number (E.164 format) and client email address entered in Settings.

---

## 2. Structure of the Notifications Tab

The screen is divided into two primary channel tabs:
1. **WhatsApp Notifications:** Powered by Meta WhatsApp Business Cloud API.
2. **Email Notifications:** Powered by transactional email services (SMTP / Cloudflare / Resend).

Under each channel, three functional sub-tabs are available:
* **Settings & Preferences:** Configure phone/email, timezone, toggles, and message type subscriptions.
* **Message History:** Audit log of all sent, delivered, read, or failed messages.
* **Manual Send:** Interactive template catalog to preview variables and manually dispatch any notification on demand.

---

## 3. Settings & Preferences Configuration

### A. WhatsApp Settings Card
* **Enable WhatsApp Notifications:** Master switch.
* **Client Contact Name:** e.g., `Rajesh Kumar` (injected into `{{first_name}}`).
* **Client WhatsApp Number:** Full international format (e.g., `+919876543210`).
* **Timezone:** Local timezone of the business.
* **Disabled Message Types:** Checkbox list allowing you to silence specific alerts (e.g., disable routine review alerts while keeping monthly reports).
* **"Send Test Message" Button:** Dispatches a test ping to verify connectivity.

---

### B. Email Settings Card
* **Enable Email Notifications:** Master switch.
* **Client Email Address:** e.g., `owner@business.com`.
* **Client Name:** Contact recipient name.
* **Disabled Email Types:** Checkbox list to silence specific email templates.

---

## 4. Complete Notification Template Catalog

The platform includes 14 standardized message templates organized across 4 categories:

| Code | Label | Category | Trigger / Purpose |
|---|---|---|---|
| **MSG_01** | Business Connected to WingerX | Onboarding | Sent immediately when onboarding a new location. |
| **MSG_02** | GBP Analysis Started | Onboarding | Sent when initial profile audit begins. |
| **MSG_03** | Initial Report Ready | Onboarding | Sent when audit finishes; includes health score. |
| **MSG_04** | What We Work On | Onboarding | Highlights top 4 focus areas from audit. |
| **MSG_05** | 90-Day Roadmap Created | Onboarding | Outlines 3-month phase milestones. |
| **MSG_06** | Task Completed | Operations | Sent when a team member marks a roadmap task complete. |
| **MSG_07** | Weekly Progress Update | Operations | Weekly performance and activity summary. |
| **MSG_08** | New Review Alert | Alerts | Immediate alert when a customer leaves a review. |
| **MSG_09** | Profile Health Alert | Alerts | Warning if profile details, hours, or photos flag issues. |
| **MSG_10** | Action Required / Approval Needed | Alerts | Notifies client if their input/approval is pending. |
| **MSG_11** | Keyword Movement | Reports | Notifies client when target keywords enter top 3/top 10. |
| **MSG_12** | Connection Problem Alert | Alerts | Sent if Google OAuth token expires or disconnects. |
| **MSG_13** | Monthly Report Summary | Reports | Monthly executive summary with impressions, calls & score. |
| **MSG_14** | 90-Day Milestone Check | Reports | Sent at Day 90 to celebrate growth and plan next quarter. |

*(The Email channel mirrors this with `EMAIL_00` through `EMAIL_14` with rich HTML templates).*

---

## 5. How to Use the Manual Send Tab

The **Manual Send** tab gives operators total control to send any notification on demand:

1. In the sidebar, click the **Notifications** tab, then select the **Manual Send** sub-tab.
2. Browse templates grouped by **Onboarding**, **Operations**, **Alerts**, and **Reports**.
3. Status indicators show whether the message has been sent previously:
   * 🟢 Green checkmark: Already sent, with timestamp.
   * ⚪ Gray circle: Not sent yet.
4. Click **"View & Send"** (or **"View & Resend"**).
5. The **Message Detail Dialog** opens with:
   * **Full Message Preview:** Live preview with real business variables interpolated.
   * **Editable Variable Values:** Verify or tweak `first_name`, `business_name`, `overall_score`, etc.
   * **Recipient Phone/Email:** Confirm recipient destination.
6. Click **"Send Message"**.
7. Toast notification confirms dispatch; record appears in **Message History**.

---

## 6. Message History Tab & Status Tracking

* **Status Values:**
  * `SENT`: Successfully handed off to the WhatsApp Cloud API / Email Gateway.
  * `DELIVERED`: Delivered to recipient device.
  * `READ`: Recipient opened and viewed the message.
  * `FAILED`: Delivery failed (e.g., invalid phone format, Meta 24-hr customer window closed).
* If a message fails, review the error description, correct the phone number or send an email fallback, and click **Resend**.
