---
itemTitle: diabetes dashboard
itemId: software-system-spec-1
itemType: Software Item Spec
itemFulfills: MPD-10
Context: Clinical
Software item type: Security
---
## Description
A safety-critical module providing clinicians and patients with a real-time, consolidated view of glucose readings, insulin dose history, dietary data, and trend analytics.

Inputs:

CGM readings (Bluetooth LE / API)
Manual blood glucose entries
Insulin dose records (basal & bolus)
Dietary/carbohydrate data
Patient configuration (target range, thresholds, units)
Authentication tokens
Outputs:

Live dashboard view (current glucose, trend arrow, time-in-range)
Glucose trend graph (24h / 7d / 30d)
Hypo/hyperglycemia alerts (<70 / >180 mg/dL)
Exportable PDF/CSV reports
JSON API payloads for downstream modules
Interfaces: Internal connections to CGM Ingestion, Insulin Pump Integration, User Profile, Auth, and Notification services; external integrations with CGM device APIs and nutrition tracking.

Rationale: Centralizes disparate data to reduce clinical cognitive load and support safe, accurate dosage decisions.
