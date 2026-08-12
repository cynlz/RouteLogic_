# Feature Roadmap, Module 4 · RouteLogic Velocity

**Team:** 2 engineers + 1 designer + 1 CS lead

## Strategic anchors
- **Persona:** Dispatch Coordinator (Desktop-based power user managing active routes, compliance, and handoffs)
- **Primary metric:** Active Cycle Time Reduction per Shift (Target: Save ≥20 mins/shift/coordinator)
- **Moment of misery:** High manual friction and repetitive data entry during compliance checks (14.6 min/step) and shift handoffs
- **Guardrail:** 0% increase in regulatory/compliance logging error rate

## Scoring
| Feature | Value | Effort | Quadrant | Decision | Rationale |
|---|---|---|---|---|---|
| B1 One-Click Compliance Checklist | 5 | 2 | Quick Win | Now | Directly attacks our primary Moment of Misery by rescuing ∼14.6 minutes per shift without violating our zero-error compliance guardrail, making it our highest-ROI anchor for the 4-week pilot |
| B2 Smart Daily Report Auto-Fill | 4 | 4 | Major Project | Next | Highly valuable operational time-saver for coordinators, but the complex AI parsing and edge case handling risks overcommitting our 2-engineer capacity during a tight 4 week pilot. |
| B3 Shift Handoff Wizard | 4 | 2 | Quick Win | Now | Solves a major coordinator friction point by systematically capturing shift handoff data, delivering a proven ∼6.8-minute daily time savings via low complexity UI flows. |
| B4 Mobile-First Coordinator Dashboard | 2 | 4 | Time Sinker | Cut | Misaligned with our primary coordinator desktop workflow, incurring heavy layout refactoring costs for minimal operational value during a 4 week pilot. |
| B5 Step Progress Indicator | 2 | 1 | Fill-In | Later | Extremely fast UI add, but provides passive process visibility rather than actively removing friction or cycle time for experienced coordinators. |
| B6 Driver Alert Notifications | 3 | 3 | Time Sinker | Cut | Serves the Driver persona rather than our primary Dispatch Coordinator, introducing mobile push infrastructure complexity that threatens our 4 week pilot timeline. |
| B7 Contextual AI ETA Display | 2 | 2 | Fill-In | Later | Low implementation effort, but inline UI placement won't drive shift velocity while base trust/adoption remains at 11% without fixing underlying model accuracy first. |
| B8 Fleet Analytics Manager View | 1 | 5 | Time Sinker | Cut | Serves executive/sales preferences with high aggregation complexity while delivering zero reduction in daily shift cycle time for our primary Dispatch Coordinator persona. |
| B9 Compliance Audit Trail Export | 1 | 3 | Time Sinker | Cut | Irrelevant for experienced power users across our 3 pilot accounts; onboarding during a 4-week pilot is far better handled directly by our dedicated CS Lead. |
| B10 In-App Coordinator Training | 1 | 3 | Time Sinker | Cut | Adds non essential software engineering bloat during a 4 week pilot; onboarding active power users across our 3 pilot accounts is far more effectively executed directly by our CS Lead. |

## Roadmap
### NOW, Pilot (4 weeks, 3 accounts)
- **B1 One-Click Compliance Checklist**, Directly attacks our primary Moment of Misery by rescuing ∼14.6 minutes per shift without violating our zero-error compliance guardrail, making it our highest-ROI anchor for the 4-week pilot
- **B3 Shift Handoff Wizard**, Solves a major coordinator friction point by systematically capturing shift handoff data, delivering a proven ∼6.8-minute daily time savings via low complexity UI flows.

### NEXT, GA Release (weeks 5-8)
- **B2 Smart Daily Report Auto-Fill**, Highly valuable operational time-saver for coordinators, but the complex AI parsing and edge case handling risks overcommitting our 2-engineer capacity during a tight 4 week pilot.

### LATER, backlog
- **B5 Step Progress Indicator**, Extremely fast UI add, but provides passive process visibility rather than actively removing friction or cycle time for experienced coordinators.
- **B7 Contextual AI ETA Display**, Low implementation effort, but inline UI placement won't drive shift velocity while base trust/adoption remains at 11% without fixing underlying model accuracy first.

### ✂ Cut List
- **B4 Mobile-First Coordinator Dashboard**, Misaligned with our primary coordinator desktop workflow, incurring heavy layout refactoring costs for minimal operational value during a 4 week pilot.
- **B6 Driver Alert Notifications**, Serves the Driver persona rather than our primary Dispatch Coordinator, introducing mobile push infrastructure complexity that threatens our 4 week pilot timeline.
- **B8 Fleet Analytics Manager View**, Serves executive/sales preferences with high aggregation complexity while delivering zero reduction in daily shift cycle time for our primary Dispatch Coordinator persona.
- **B9 Compliance Audit Trail Export**, Irrelevant for experienced power users across our 3 pilot accounts; onboarding during a 4-week pilot is far better handled directly by our dedicated CS Lead.
- **B10 In-App Coordinator Training**, Adds non essential software engineering bloat during a 4 week pilot; onboarding active power users across our 3 pilot accounts is far more effectively executed directly by our CS Lead.
