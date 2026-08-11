# Hypothesis & Success Metrics (Module 3)

## Pre-work · Hypothesis check
- **Role , who you are solving for (from M2):** We are solving for the dispatcher directly satisfies the Fleet Driver (better routes) and delivers the business ROI required by the Logistics Manager (the buyer).
- **Goal , what this user is ultimately trying to achieve:** The user is trying to transform an error prone, high-stress morning ritual into an automated, single pane of glass workspace that lets them dispatch their fleet with speed, precision, and confidence
- **Friction / moment of misery , the specific pain blocking their goal:** The dispatcher is trapped acting as a human middleware engine wasting hours manually stitching together disconnected, non-commercial tools to build routes that still fail in the real world, causing constant missed SLAs and high operational stress.
- **Current workaround , the external tool or manual process they rely on (M2):** To bypass the tool's data gap, the dispatcher acts as the human middleware, manually stitching together Excel for stop assignment, Google Maps browser tabs the route  estimation  and SMS for driver communication.
- **Problem Hook , your one-sentence framing of the business crisis (M1):** Managers are trapped in hours of manual spreadsheet workarounds, driving up operational costs and putting client SLAs and our market credibility at immediate risk.
- **Value Proposition , the outcome your initiative promised to deliver (M1):** This approach eliminates manual dispatch hacks by delivering an automated, data driven routing workspace that cuts operational planning from hours to minutes, reduces fleet cost per mile, and guarantees enterprise delivery SLAs.

## Read your data snapshots
- **Does the funnel data confirm your M2 friction point, or does it tell a different story? Note where the numbers align with the qualitative pain you found and where they diverge.:** _(not filled in)_
- **Do the retention patterns align with the workaround your M2 persona used to find content? Note what the Mo. 0→1 drop suggests about the onboarding experience your persona described as frustrating.:** _(not filled in)_
- **Does the LTV gap and the content mix (61% trending for Wanderers) confirm the moment of misery your persona described? Note which segment your persona is in and whether the data confirms their pain.:** _(not filled in)_
- **Does the low adoption confirm your persona is burdened by tools they don’t use? Note whether the low scheduling adoption (42%) for coordinators matches your M2 moment of misery.:** 1. Feature Burden Confirmation
Yes. Frontline personas (Drivers & Coordinators) are burdened by unused bloat.
Core Focus: Frontline activity clusters heavily on just 3 features (Live Dispatch, Route Optimizer, and Compliance Checklist—all 64%+ adoption).
Feature Bloat: High-investment features like AI Predictive ETAs sit essentially unused (11% Drivers, 23% Coordinators).
Takeaway: Forcing frontline power users through enterprise features tailored for Managers creates visual and operational friction, cluttering their daily core workflow.
2. Shift Scheduling (42%) vs. M2 "Moment of Misery"
Yes. The 42% Coordinator adoption rate validates the M2 moment of misery.
The Disconnect: While Managers heavily use Shift Scheduling (79%), over half of Coordinators (58%) abandon it.
- **Does the workflow data match the manual process or hack you documented in M2? Note whether the specific drop-offs or time gaps explain why your persona avoids the digital tool.:** 1. Alignment with M2 Manual Hack
Yes. The workflow data directly validates the manual workarounds documented in M2.
Workflow Collapse: Completion drops sharply from 71% at Assign Routes down to 48% at Log Compliance Checks, with a 69% cumulative abandonment rate after route assignment.
The "Hack" Confirmed: Coordinators rely on the tool only for route generation, then immediately abandon the platform mid-workflow to handle compliance logging, shift handoffs (31% completion), and daily reporting (18% completion) via external manual hacks (e.g., spreadsheets, paper logs, side messaging).
2. Why the Persona Avoids the Digital Tool
Extreme time gaps directly explain why Coordinators abandon the native workflow:
Massive Compliance Bottleneck: Log Compliance Checks takes 14.6 minutes vs. a 3-minute benchmark (+11.6 min gap / nearly 5× longer), creating immense friction that triggers initial abandonment.
Compounded Time Waste: Later steps—Complete Shift Handoff (+6.8 min gap) and File Daily Report (+6.7 min gap)—are also more than double benchmark expectations, totaling 31 minutes of daily wasted time.
- **Look at the CSAT heatmap. Which specific cell most directly maps to your persona’s friction? Note how the NPS trend justifies the urgency of your M1 Problem Hook.:** Primary Cell: Coordinators × Compliance (CSAT 2.2 / "Weak")
Direct Friction: While Coordinators × Scheduling (2.6) is also weak, the Compliance cell (2.2) represents the lowest-rated daily task area that Coordinators are required to execute.
The Connection: This directly aligns with Snapshot 2, where logging compliance checks caused the largest bottleneck (14.6 min vs. 3 min benchmark), driving Coordinators away from the native tool and into manual hacks.
2. NPS Trend & Urgency for M1 Problem Hook
The 30-Point NPS Collapse (+18 down to -12) proves immediate business urgency.
Escalating Wasted Time: Coordinator time lost to manual workarounds has surged 3.4× (from ~9 min to 31 min daily).
Churn Risk: Product complexity is now driving 4 out of 5 account churns (up from 1 in 8 two years ago).

## Step 3 · Craft your hypothesis
- **Qualitative evidence (from M2) , quote the specific friction / moment of misery for your persona:** Coordinators are forced into manual, off-platform workarounds, losing 31 minutes daily—due to extreme workflow friction in Compliance Logging  and Shift Scheduling, where 69% abandon the digital tool mid process.
- **Quantitative evidence (from M3) , name the metric or data point that confirms the pain; cite the number:** Quantitative Evidence (from M3)
Primary Bottleneck Metric: Compliance Check completion time takes 14.6 minutes vs. a 3.0-minute benchmark (+11.6 min gap / nearly 5× longer).
Workflow Abandonment: A 69% cumulative drop-off rate occurs after route assignment, leading to only 31% completing Shift Handoff and 18% filing Daily Reports.
Operational Impact & Sentiment: Time lost to manual workarounds reached 31 minutes daily (a 3.4× increase), driving a 30-point NPS collapse for Coordinators (dropping from +18 to -12) and contributing to 4 out of 5 accounts citing complexity as their churn reason.
- **Persona , role, goal, and the friction you confirmed in the reconciliation steps:** Role: Operations Coordinator (RouteLogic Frontline Power User)
Goal: Execute daily dispatch operations smoothly—assigning routes, logging compliance, and completing shift handoffs—without losing time or disrupting live workflows.
Confirmed Friction: Severe workflow inefficiency in core admin tasks—specifically Compliance Checks (14.6 min vs. 3 min benchmark)—causing a 69% workflow abandonment rate and forcing them into manual workarounds that waste 31 minutes daily.
- **Problem you are solving , one sentence describing the specific friction this initiative removes:** This initiative streamlines the high-friction compliance logging and shift handoff processes within RouteLogic to eliminate 31 minutes of daily wasted time and prevent off-platform manual workarounds for Operations Coordinators.
- **Strategic outcome , what behaviour change do you expect, and how does it map to retention / revenue / churn?:** Expected Behavior Change: Operations Coordinators will complete compliance checks and shift handoffs directly within RouteLogic instead of abandoning the platform for off-platform manual workarounds (driving workflow completion above the current 31% baseline).
Impact on Retention, Revenue, and Churn: Eliminating the 31 minutes of daily wasted time directly addresses the core complexity driving 4 out of 5 account churns, reversing the Coordinator NPS collapse (-12) and protecting recurring B2B software revenue by improving account retention.
- **Primary success metric (initiative signal) , the leading indicator that tells you the gap is closing:** Leading Indicator: Average time spent on Compliance Checks (targeting a drop from 14.6 minutes down toward the 3.0-minute benchmark).
Why it Signals Success: Reducing this specific bottleneck is the earliest proof that friction is removed, directly driving an increase in full workflow completion (from 31% baseline) before lag metrics like CSAT, NPS, or churn show results.
- **Guardrail metric (product signal) , the metric that must NOT drop; it protects your existing base:** Metric to Protect: Core Dispatch & Route Optimizer Daily Active User (DAU) Adoption (currently at 91% for Coordinators and 88% for Drivers).
Why It Must Not Drop: These core features represent the frontline power users' primary daily workflow; simplifying compliance and handoffs must not add friction, latency, or complexity to the essential route planning and live dispatch operations that keep daily fleet performance intact.
- **Decision window , how much time or data before you scale, pivot, or kill? minimum threshold to proceed?:** Timeframe / Sample Size: 2 to 4 weeks post-launch (or after tracking a minimum of 500 completed coordinator dispatch workflows).
Minimum Threshold to Proceed (Scale):
Compliance check completion time drops from 14.6 minutes to ≤ 5.0 minutes.
Workflow completion rate through Shift Handoff increases from 31% to ≥ 60%.
Pivot / Kill Trigger: If compliance logging time remains above 10.0 minutes or guardrail metrics (Dispatch/Optimizer DAU) drop by >5%, pause rollout to iterate on UX or pull the initiative.
- **Draft your full hypothesis sentence , one to three sentences; quote the metric, name the persona, name the outcome:** Based on qualitative findings of manual workarounds and quantitative evidence showing a 69% workflow abandonment rate driven by a 14.6-minute compliance bottleneck, I believe that streamlining the compliance logging and shift handoff workflows for Operations Coordinators will result in eliminated off-platform workarounds and reduced account churn, as measured by a >60% reduction in average compliance check completion time (dropping from 14.6 to ≤5.0 minutes). I will protect Core Dispatch and Route Optimizer DAU adoption (≥91%) and will make a go/no-go decision after 2 to 4 weeks (or 500 completed workflows).
