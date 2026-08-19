# GTM Launch Plan, RouteLogic (B2B)

| Field | Value |
|---|---|
| Feature | Automated Compliance Logging & Digital Shift Handoff Module |
| Goal | Conversion |
| Launch tier | M, Targeted |

## Goal & Audience
- **Goal:** Conversion, Addresses Immediate Value Realization: In M5 testing, the feature proved it cuts compliance logging time from 14.6 minutes down to 3.2 minutes. The primary bottleneck isn't getting users to know the app exists (awareness) or browse around (engagement); it is driving active conversion away from off-platform spreadsheets into full in-app workflow completion.
Directly Eliminates Churn Risk: The 69% baseline workflow abandonment rate represents a critical leak in product utility. Securing conversion on this specific handoff feature converts high-friction, frustrated accounts into retained, sticky users.
Lowers Operational Friction Fast: Because these are existing RouteLogic users, driving conversion immediately unlocks the efficiency gains validated in the pilot without requiring a multi-stage acquisition top-of-funnel campaign.
- **Target audience:** Operations Coordinators at Existing Active Accounts with High Workflow Abandonment
Segment Definition: Active Operations Coordinators at current B2B enterprise accounts who handle daily driver dispatch and shift handoffs, but currently exhibit ≤31% in-app workflow completion due to reliance on manual, off-platform spreadsheets for compliance tracking.
Key Characteristics: High-volume daily users of RouteLogic’s Core Dispatch and Route Optimizer features, but frustrated by the 14.6-minute administrative compliance bottleneck.

## Launch Tier
- **M, Targeted**, Launch Tier Justification (Tier M: Targeted)
Reach: Focuses strictly on the active Operations Coordinator segment across existing B2B enterprise accounts—specifically targeting the subset displaying low in-app completion rates (≤31%) without distracting unaffected account tiers.
Revenue Impact: Protects net revenue retention (NRR) by directly eliminating the administrative compliance friction driving account dissatisfaction and churn risk, rather than driving new top-of-funnel acquisition revenue.
Risk of Silence: High operational risk if silent. If coordinators are not actively guided and enabled through the new workflow, they will default to their ingrained habits (manual off-platform spreadsheets), rendering the product improvement unused and leaving churn risks unresolved.

## Channels
1. **Owned: In-App Guidance & Product Tours (Appcues / Pendo Walkthroughs) Channel Type: Owned Why It Reaches Your Audience: Operations Coordinators spend their entire workday logged directly into the RouteLogic web app running live dispatches. Reaching them in-context at the exact moment they enter the compliance or shift handoff workflow eliminates channel friction, capturing their attention directly within their active workspace. Mechanism: Triggered interactive tooltips and modal banners that launch automatically for targeted coordinators showing low completion history, guiding them through the 2-tap compliance process step-by-step.**
2. **Owned: Direct Targeted Email & CSM Outreach Campaigns Channel Type: Owned Why It Reaches Your Audience: Operations Coordinators and fleet managers rely heavily on email for daily account communications, system alerts, and operational updates. Mechanism: Triggered email sequences sent to designated account admins and low-completion coordinators highlighting time savings (cutting logging from 14.6 to 3.2 minutes), paired with direct Customer Success Manager (CSM) outreach for key B2B accounts during weekly review syncs.**
3. **Owned: RouteLogic Knowledge Base & Customer Help Center Channel Type: Owned Why It Reaches Your Audience: Operations Coordinators actively seek self-service documentation and video guides when onboarding new team members or troubleshooting daily compliance workflows. Mechanism: Short, step-by-step video tutorials (≤90 seconds) and updated SOP articles embedded directly in the Help Center, demonstrating how to use the 2-tap compliance flow and complete digital shift handoffs.**

## Enablement & Assets
Enablement Brief & Assets
Sales / Customer Success Enablement:
Needs a clear value framework linking the 11.4-minute time savings per shift to net revenue retention (NRR) and reduced churn risk.
Talking points to handle coordinator resistance to changing manual habits during regular account reviews.
Support Team Enablement:
Internal troubleshooting matrix for BLE/Auto-populate compliance logging failures.
Standardized response macros to resolve common user questions without escalating to product engineering.
Key Assets to Build:
1-Page Customer Value Sheet (PDF): A concise summary detailing the shift handoff workflow benefits, showing how the module eliminates 11+ minutes of daily admin work.
90-Second Product Demo Video: A quick screen recording demonstrating the 2-tap compliance logging and digital handoff screen in action.
Interactive Walkthrough Script: A step-by-step Pendo/Appcues guide embedded directly into the CSM account review playbook.

## Ownership, Budget & Timeline
- **Ownership & budget:** GTM Lead & Execution Owner: Jane Doe (Product Manager) – Overall launch coordination, timeline tracking, and metric alignment.
In-App Tour & Walkthrough Build: Alex Smith (Product Marketing Manager) – Designing, testing, and deploying Pendo/Appcues flows.
CSM & Sales Enablement Playbook: Marcus Vance (Customer Success Lead) – Drafting CSM talk tracks, account targeting list, and running internal CS training.
Support Knowledge Base & Macros: Sarah Jenkins (Customer Support Specialist) – Authoring Help Center articles, video scripts, and support macros.
Demo Video & Asset Creation: David Chen (Visual/Content Designer) – Producing the 1-page PDF value sheet and 90-second demo video.
- **Timeline:** Phase 1: Beta & Pre-Launch Enablement (Weeks 1–2)
Build & Test In-App Tours: Alex Smith configures and QA-tests Pendo walkthrough flows for the target segment.
Team Enablement: Marcus Vance trains CSMs using the new talking points; Sarah Jenkins publishes internal support macros.
Asset Finalization: David Chen creates the 1-Page Value Sheet, and Alex Smith records the narrated Loom product demo.
Phase 2: Launch Moment & Targeted Rollout (Week 3)
Feature & Tour Activation: Jane Doe switches on the Automated Compliance & Shift Handoff module alongside in-app Pendo tours for targeted accounts.
Direct Outreach: CSMs initiate outreach to low-completion B2B enterprise accounts; triggered email announcements launch.
Knowledge Base Live: Sarah Jenkins publishes public-facing Help Center articles and step-by-step videos.
Phase 3: Post-Launch Optimization & Account Nurture (Weeks 4–6)
Adoption Tracking: Jane Doe monitors weekly in-app completion metrics (targeting ≥60% completion rate).
Support Sweep & Feedback: CSMs gather qualitative feedback during account syncs; Sarah Jenkins reviews support ticket volume to refine macros.
Tour Iteration: Alex Smith optimizes drop-off points within the in-app guidance based on Pendo interaction analytics.

## Success Metrics
- **Metrics:** 1. Core Success Metric: Target Segment Workflow Completion Rate
The Metric: Percentage of shift handoff sessions where the targeted low-completion coordinator segment executes compliance logging in-app rather than abandoning the flow.
Target: Increase from 31% baseline to ≥60% within 4 weeks post-launch.
Bad Signal: Completion rate stays stuck below 40% despite high Pendo walkthrough views.
Actionable Next Step: If users are starting the tour but abandoning the flow midway, the 2-tap UI contains friction or a bug (e.g., auto-populate BLE connectivity drops); trigger direct CSM account interviews and review session recordings via PostHog/FullStory.
2. Time-to-Complete Metric: Average Compliance Logging Duration
The Metric: Total active seconds spent by a coordinator logged into the compliance module per shift.
Target: Maintain an average of ≤3.5 minutes per coordinator shift (matching the M5 experiment benchmark of 3.2 minutes, down from 14.6 minutes).
Bad Signal: Average time creeps back above 8.0 minutes.
Actionable Next Step: Indicates coordinators are manually overriding pre-filled data or experiencing system latency; pause automated prompts, deploy a quick fix to the pre-fill logic, and publish targeted support macros addressing the manual override confusion.
3. Critical Guardrail Metric: Core Dispatch DAU & Operational Speed
The Metric: Daily Active Users (DAU) and average task duration on the core Route Optimizer/Dispatch screen.
Target: Keep Core Dispatch DAU steady at ≥91% and active dispatch task time unchanged.
Bad Signal: Core Dispatch DAU drops below 88% or average dispatch assignment time increases by >15%.
Actionable Next Step: The new compliance module or Pendo modal overlay is blocking or slowing down core dispatch operations; immediately suppress broad in-app banners, revert the modal trigger to a soft inline notification, and unblock the primary dispatch UI.
- **Bad signal to watch for:** High Tour Engagement, Low Workflow Completion (≥70% View Rate, <40% Completion) The Diagnosis: Value proposition clear, execution friction high. What It Means: Coordinators are interested in the feature, but the product UI or data pre-fill mechanics fail mid-task (e.g., auto-populate drops BLE signal or errors out). Next Action: Pause marketing messaging and trigger immediate product usability testing / FullStory session reviews to fix the UI blocker. High In-App Drop-Off + Manual Overrides (>30% Manual Edits) The Diagnosis: Lack of trust in automated data. What It Means: Coordinators don't trust the pre-filled compliance metrics and spend 8+ minutes re-checking and manually editing fields, defeating the purpose of the 2-tap flow. Next Action: Have CSMs run direct enablement sessions showing data accuracy proofs, and update the 1-page value sheet to address data verification trust. Declining Core Dispatch DAU (<88% Core Dispatch Adoption) The Diagnosis: Intrusive enablement blocking core workflow. What It Means: The new Pendo modals or compliance alerts are interrupting live dispatch actions, causing frustration and forcing coordinators to close the app. Next Action: Immediately kill modal popups; shift to soft, passive banners or inline notifications within the dispatch interface.
- **Likely post-launch decision:** Iterate  Primary Trigger The Diagnostic Signal: High Pendo walkthrough adoption (≥70%) paired with moderate workflow completion (40%–55%), missing our 60% conversion target. The Root Cause: Coordinators see the value and start the flow, but experience localized friction—such as auto-populate data delays or lingering distrust in pre-filled compliance metrics—causing them to drop back into manual spreadsheet habits. Actionable Path Ahead If We Iterate (Most Likely): Product Adjustment: Refine pre-fill accuracy, optimize UI micro-copy (e.g., adding a quick "Verify & Submit" confirmation prompt), and adjust Pendo modal timing so it doesn't interrupt live dispatch actions. Enablement Shift: Deploy short, targeted CSM Loom walkthroughs to low-completion accounts demonstrating data verification accuracy. What Would Force a Pivot or Deprioritization Instead? Pivot Trigger: Completion stays stuck below 31% while Core Dispatch DAU drops below 88%. This indicates the feature fundamentally disrupts active dispatch operations, forcing a redesign from a standalone module into a passive background auto-logger. Deprioritize Trigger: Completion reaches 60%+ within 2 weeks with near-zero support ticket friction. The core conversion problem is solved, allowing product and engineering resources to reallocate to the next high-impact roadmap item.
