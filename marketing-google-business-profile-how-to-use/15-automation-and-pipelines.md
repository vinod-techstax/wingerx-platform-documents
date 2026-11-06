# Automation, Pipelines & Schedules

The **Automation** tab (encompassing **Pipelines**, **Pipeline Runs**, and **Schedules**) powers autonomous marketing workflows. It enables multi-step execution chains (e.g., Run Audit → Generate Posts → Draft Review Replies → Send Notification) on set recurring schedules.

> **Navigation:** Go to https://app.wingerx.com/marketing page and click the **Automation** tab.

---

## 1. Core Concepts
* **Pipeline:** A configured sequence of automated steps (e.g., `Weekly Content Generation Pipeline`).
* **Step Types:** Audit execution, keyword discovery, post draft generation, review reply generation, notification dispatch.
* **Pipeline Run:** A single execution of a pipeline, recording execution status per step with full input/output logs.
* **Schedule:** A cron or timer trigger that executes a pipeline automatically (e.g., every Tuesday at 09:00 AM).

---

## 2. Key Components & How to Use Them

### A. Creating a Pipeline
1. In the sidebar, click the **Automation** tab.
2. Click **"New Pipeline"**.
3. Name your pipeline (e.g., *"Bi-Weekly GBP Content Engine"*).
4. Add Steps:
   * **Step 1: Check Reviews** — Scan for newly received reviews and draft replies.
   * **Step 2: Generate Post** — Create a What's New post targeting approved keywords.
   * **Step 3: Submit to Queue** — Route all outputs to the **Approval Queue** tab.
5. Save the pipeline.

---

### B. Triggering a Pipeline Run
1. Select the target pipeline and click **"Run Pipeline"**.
2. Monitor real-time step progress (Pending → Running → Completed).
3. Inspect step output payloads, token usage, and any errors.

---

### C. Configuring Recurring Schedules
1. Switch to the **Schedules** sub-tab.
2. Click **"Add Schedule"**.
3. Select the pipeline, execution frequency (Daily, Weekly, Monthly), day of the week, and local time.
4. Toggle schedule **Active**.
