# Approval Queue & Safety Governance

The **Approval Queue** is the mandatory governance gate where all AI-generated content (Google Posts, review replies, blog articles, and profile updates) is reviewed by human operators before going live to prevent hallucinated claims, unauthorized promises, or brand compliance violations.

> **Navigation:** Go to https://app.wingerx.com/marketing page and click the **Approval Queue** tab.

---

## 1. Prerequisites
- A location or workspace must be selected.
- The sidebar displays a dynamic badge count showing the number of pending items (e.g., `3`).

---

## 2. Key Components & How to Use Them

### A. Risk Level Filtering & Badges
Every generated item is automatically analyzed by the governance engine and assigned a risk tier:
* 🟢 **Low Risk:** Standard greeting, review reply matching predefined rules, routine holiday hours notice.
* 🟡 **Medium Risk:** Promotional offer with pricing or discount terms, service change, new photo upload.
* 🔴 **High Risk:** Medical claims, legal advice, guarantee statements, negative review dispute response.

---

### B. Action Controls
On each approval card:
1. **Approve:** Authorizes the action. If the location is OAuth-connected, the item is immediately dispatched to Google APIs.
2. **Edit:** Opens the inline editor to revise text, change CTA buttons, or replace attached photos before approving.
3. **Reject:** Dismisses the generated item with optional feedback to train future AI prompts.
4. **Complete Manually:** Specially designed for non-OAuth (Google Places managed) locations. After posting the update manually to Google Maps, clicking this moves the item to completed status and logs it in the **Audit Log** tab.

---

### C. Batch Actions
* Use checkboxes to select multiple low-risk review replies or standard updates.
* Click **"Batch Approve Selected"** to process routine tasks in seconds.
