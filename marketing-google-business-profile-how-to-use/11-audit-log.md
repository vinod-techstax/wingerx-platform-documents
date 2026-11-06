# Audit Log & Compliance History

The **Audit Log** tab provides an immutable, chronological event ledger of every marketing activity, AI generation, human approval, manual edit, notification dispatch, and profile modification performed across the location.

> **Navigation:** Go to https://app.wingerx.com/marketing page and click the **Audit Log** tab.

---

## 1. Why the Audit Log is Essential
* **Client Transparency:** Answers *"Who published this post?"*, *"When was this review replied to?"*, and *"Which operator approved this change?"*.
* **Regulatory & Brand Compliance:** Provides full traceability for healthcare, legal, real estate, and financial businesses where published claims are regulated.
* **Troubleshooting:** Helps diagnose sync issues, failed webhook dispatches, or unexpected profile changes.

---

## 2. Key Components & How to Use Them

### A. Filter & Search Controls
* **Filter by Action Type:** `Content Created`, `Content Approved`, `Post Published`, `Review Answered`, `Notification Sent`, `Setting Changed`.
* **Filter by Actor:** System / AI Automations vs. Specific User Team Members.
* **Date Range:** Filter events within a specific calendar window.

---

### B. Event Record Details
Each log entry displays:
* **Timestamp:** Exact date and time (adjusted to local timezone).
* **Actor:** User name, email, or `WingerX Automation Engine`.
* **Action:** Clear event label (e.g., `APPROVED_POST`, `SENT_WHATSAPP_MSG_01`).
* **Target Resource:** ID and title of the post, review, or notification.
* **Payload Diff:** Before-and-after snapshot if a setting or copy was edited.
