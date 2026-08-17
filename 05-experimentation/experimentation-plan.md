# A/B Experiment Brief, RouteLogic (B2B)

## Parameters
| Parameter | Decision |
|---|---|
| Feature under test | Feature B1 · One-Click Compliance Checklist |
| Persona | Primary User Role: Dispatch Coordinators responsible for verifying daily shift logs, driver credentials, vehicle inspection data, and route execution before/after shifts. Core Pain Point Addressed: High administrative drag and daily operational friction caused by manual data re-entry (14.6 minutes spent per shift on compliance logs). Sample Unit: Individual Completed Shift Compliance Review Events handled by coordinators across the pilot fleets during the 4-week test window. |
| Expected outcome | Primary Outcome: A drastic reduction in active time spent per shift compliance review from 14.6 minutes down to under 60 seconds, while maintaining a strict 0% regulatory error rate. Behavioral Shift: Dispatch coordinators transition from tedious, manual data entry and cross-referencing to an exception-based review and one-click verification workflow. Instead of typing repetitive driver, route, and vehicle details, coordinators effortlessly scan pre-filled telemetry (≥80% auto-filled), quickly resolve any amber-highlighted delta fields, and finalize audit-locked logs instantly using single clicks or desktop hotkeys (Cmd/Ctrl + Enter). |
| Primary success metric | Active Compliance Verification Cycle Time per Shift (Target: Drop from 14.6 mins to <1.0 min) |
| Baseline rate | Current Active Compliance Verification Cycle Time: 14.6 minutes per shift review (with a 0% compliance logging error rate baseline). |
| Guardrail metric | Compliance Logging Error Rate (Target: Strict 0% Error Rate) |
| Guardrail boundary | Strict 0% Compliance Logging Error Rate (Zero unvalidated form submissions, missing regulatory fields, or audit log failures). Hard Operational Ceiling: If the Variant experiences >0.0% regulatory errors or >2% technical submit failures (e.g., API payloads failing to generate SHA-256 audit logs or missing mandatory driver fields), the experiment will be immediately paused or rolled back. |
| Second guardrail | Guardrail Metric: Shift Dispatch Hold Time / Board Bottleneck Rate Threshold / Boundary: ≤0% increase in delayed shift departures (Zero net increase in fleet dispatch delays caused by coordinator workflow disruption or UI confusion). Distinct Harm Protected: While Guardrail 1 (0% Regulatory Error Rate) protects against legal and compliance risk, Guardrail 2 protects against operational downstream friction. It ensures that adopting a new verification interface does not inadvertently slow down physical fleet departures or cause dispatch board bottlenecks if a coordinator encounters UI confusion or input friction. |
| Minimum Detectable Effect | MDE Target: 80% Reduction in Cycle Time (a reduction of ≥11.68 minutes per shift review). Target Shift Review Time: Dropping from the 14.6-minute baseline down to ≤2.92 minutes (with an ultimate target of <60 seconds in the Variant). |
| Sample size per arm | Total Sample Size Across Both Arms: ≈240 completed shift compliance logs. |
| Traffic split | 50% Control: Legacy manual data entry workflow (14.6-minute baseline). 50% Variant: Feature B1 One-Click Compliance Checklist workspace (≥80% pre-filled). |
| Test duration | 4 Weeks (20 business operational days) |
| Significance threshold | p<0.05 (95% Confidence Level, 2-tailed test) |

## Control vs. Variant
- **Control (A):** Control (A) — The Status Quo Experience
Workflow Description: The legacy manual shift verification process. Coordinators must manually open raw dispatch logs, copy-paste or re-key driver IDs, route codes, vehicle registrations, and pre-trip inspection statuses across disconnected forms/spreadsheets.
Moment of Misery: An agonizing 14.6-minute manual data entry step per shift—cross-referencing logs, re-keying driver details, and risking regulatory fines with every manual entry.
Baseline Output:
Mean Cycle Time: 14.6 minutes per shift review.
Friction Points: High administrative drag, manual re-entry fatigue, and human data converter bottleneck.
- **Variant (B):** Variant (B) — The One-Change Transformation (Feature B1)
The Variant introduces Feature B1: One-Click Compliance Checklist, replacing manual form completion with an automated workspace that pre-fills ≥80% of compliance fields directly from active dispatch payloads.
Screen 1 — Entry Point: Dispatch Dashboard (Pre-Submission)
Purpose: Surface the active compliance task seamlessly within the Coordinator's existing desktop shift workflow.
Key UI Elements:
Alert Banner / Status Card: Prominent visual badge reading "Shift Compliance Review Ready (1 Pending)".
Quick Metrics Summary: High-level shift details (Driver Name, Vehicle #, Route ID) with a secondary label showing "Auto-filled from Shift Data".
Primary Call-to-Action (CTA): High-contrast button reading [ Review & Sign Off (14m saved) ] that opens the compliance modal or transitions to Screen 2.
Screen 2 — Feature Core: Smart Pre-Filled Compliance Workspace
Purpose: Where the 14.6-minute friction is collapsed into a <60-second review.
Key UI Elements:
80%+ Pre-Filled Fields: Form fields (Driver ID, Hours of Service, Pre-Trip Inspection, Vehicle Reg) rendered in a "Verified" state with subtle green check icons.
Delta Highlighting: Any missing or unverified mandatory field rendered in an active amber/warning outline (e.g., "Missing Odometer Reading"), auto-focusing the cursor.
Primary Action Footer: Fixed bottom bar housing:
Primary Button: [ Verify & Submit Checklist (Cmd + Enter) ] (Disabled if mandatory delta fields are empty).
Hotkey Indicator: Subtle Tab / Cmd + Enter visual tags for power-user desktop velocity.
Screen 3 — Success / Confirmation: Immutable Audit Sign-Off
Purpose: Provide immediate visual feedback that the shift is compliant and locked, protecting our 0% error rate guardrail.
Key UI Elements:
Confirmation Card: Green success banner reading "Shift #4082 Compliance Locked & Submitted".
Audit Metadata Stamp: Displayed details: Timestamp (e.g., 07:01:14 AM), Coordinator ID, and Immutable Hash #.
Time Saved Indicator: Toast notification reading "⚡ Completed in 28 seconds — 14.1 minutes saved this shift."
Next Steps CTA: Secondary button [ Return to Active Fleet Map ] to seamlessly transition back to live dispatching.
- **Held constant (isolation check):** Target Users & Context: The exact same pool of Dispatch Coordinators reviewing live shifts across the same 3 pilot enterprise accounts during active shift hours.
Underlying Regulatory Requirements: The mandatory compliance parameters (Driver ID, Hours of Service, Pre-Trip Inspection, Vehicle Registration, Odometer Reading) required for shift sign-off are unchanged.
Backend Database & Audit Ledger Structure: Both arms write to the same compliance ledger database and require the exact same SHA-256 audit logging and ISO-8601 timestamping formats upon submission.
Shift Initialization & Triggering Conditions: Shifts are initialized at the exact same times using the exact same underlying dispatch session triggers and payloads.
Success Criteria & Guardrail Thresholds: The core definition of a compliant shift and the 0% error tolerance policy apply equally to both arms.
The Single Variable Changed
The Interface & Input Layer: Transitioning from manual, multi-field data entry (Control) to an automated, ≥80% pre-filled compliance workspace with delta highlighting and desktop hotkey sign-off (Variant).

## Hypothesis
> I believe that Feature B1 · One-Click Compliance Checklist for Primary User Role: Dispatch Coordinators responsible for verifying daily shift logs, driver credentials, vehicle inspection data, and route execution before/after shifts. Core Pain Point Addressed: High administrative drag and daily operational friction caused by manual data re-entry (14.6 minutes spent per shift on compliance logs). Sample Unit: Individual Completed Shift Compliance Review Events handled by coordinators across the pilot fleets during the 4-week test window. will result in Primary Outcome: A drastic reduction in active time spent per shift compliance review from 14.6 minutes down to under 60 seconds, while maintaining a strict 0% regulatory error rate. Behavioral Shift: Dispatch coordinators transition from tedious, manual data entry and cross-referencing to an exception-based review and one-click verification workflow. Instead of typing repetitive driver, route, and vehicle details, coordinators effortlessly scan pre-filled telemetry (≥80% auto-filled), quickly resolve any amber-highlighted delta fields, and finalize audit-locked logs instantly using single clicks or desktop hotkeys (Cmd/Ctrl + Enter)., as measured by a MDE Target: 80% Reduction in Cycle Time (a reduction of ≥11.68 minutes per shift review). Target Shift Review Time: Dropping from the 14.6-minute baseline down to ≤2.92 minutes (with an ultimate target of <60 seconds in the Variant). change in Active Compliance Verification Cycle Time per Shift (Target: Drop from 14.6 mins to <1.0 min) within 4 Weeks (20 business operational days). We will protect Compliance Logging Error Rate (Target: Strict 0% Error Rate) throughout the test.

## Shipping criteria
> We will **ship** if Active Compliance Verification Cycle Time per Shift (Target: Drop from 14.6 mins to <1.0 min) improves by ≥ MDE Target: 80% Reduction in Cycle Time (a reduction of ≥11.68 minutes per shift review). Target Shift Review Time: Dropping from the 14.6-minute baseline down to ≤2.92 minutes (with an ultimate target of <60 seconds in the Variant). at p<0.05 (95% Confidence Level, 2-tailed test) and Compliance Logging Error Rate (Target: Strict 0% Error Rate) does not reach Strict 0% Compliance Logging Error Rate (Zero unvalidated form submissions, missing regulatory fields, or audit log failures). Hard Operational Ceiling: If the Variant experiences >0.0% regulatory errors or >2% technical submit failures (e.g., API payloads failing to generate SHA-256 audit logs or missing mandatory driver fields), the experiment will be immediately paused or rolled back. after 4 Weeks (20 business operational days).
> We will **iterate** if direction is positive but lift is below the MDE.
> We will **kill** if the primary metric shows no improvement or moves negatively.
> The read date is fixed at the end of 4 Weeks (20 business operational days), no results reviewed before this date.
