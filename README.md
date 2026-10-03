# Hi, I'm Agnidh Ghosh

I work in the founder's office at 30 Sundays, a travel tech startup backed by Info Edge and Bessemer Venture Partners, where I own revenue analytics and program management end to end. I take the questions leadership and the sales org actually ask, decide what gets built and in what order, turn them into numbers people can trust, and ship the tools that put those numbers in front of the right person while a decision is still open.

Below are selected systems I have designed, built, and run in production. The code and the data stay private. What follows is a description of the work and the thinking behind it.

## How the work runs

Most of what I do is a loop, and I own all of it. This is program management as much as engineering: I decide what gets built and in what order, not only how.

1. **Intake.** Requests come from the CBO, business heads, managers, and team leads. I built a small intake app so those requests land in one place with context, instead of scattered across chats.
2. **Prioritize.** I decide what gets built, what waits, and what is actually a data-quality problem wearing a feature request as a costume.
3. **Build and validate.** I write the pipelines and the dashboards, then reconcile every number against the existing source of truth before anyone sees it.
4. **Ship and maintain.** Each tool is live, used daily, and carries its own monthly rollover, access control, and failure handling.

The part that matters most is step three. A dashboard that is pretty and wrong is worse than no dashboard, because people act on it.

## Selected systems

**Sales performance dashboards (three business units, down to every seller).**
Everyone in the sales org needed to see how they were tracking against target, from the business head down to the individual seller. I built role-scoped dashboards across all three business units and their destinations: a business head sees the whole unit, a team lead sees their team, and a seller sees their own numbers, including the incentive they are on track to earn, so the target is something they can act on.

**Weekly seller review.**
Weekly reviews work best when the time goes into coaching, not into preparing numbers. I built a weekly review tool that has the numbers ready in advance and shows, per seller, where the funnel is leaking and what to do about it. It reads the same figures as the business-unit dashboard, so sellers, managers, and leadership all work from one set of numbers.

**Diagnostic deep-dives.**
A headline number tells you something is wrong. It does not tell you where, for whom, or what to do next. I built drill-downs that go from a team's aggregate all the way down to a single lead's journey: where it stalled, whether it was ever called, how long the first response took, whether an itinerary was sent and then went quiet. The point is to turn "conversion is down" into "these specific leads stalled at this exact step, and here is the one thing to fix." It also surfaces work that is otherwise invisible, like itineraries built while a lead was wrongly marked lost, so effort gets credited and problems get caught early.

**Supply analytics and NPS.**
The supply team needed to see what we buy, how it performs, and what customers think of it. I built a supply dashboard on live booking data that shows which hotels, activities, and partners are actually sold and used, so contracting decisions rest on real demand. It also reads every NPS comment with an LLM, labels the issue and the team that owns the fix, and traces it to the exact hotel or activity, so a falling score becomes a short list of fixes.

**Leadership view.**
The CXO team needed revenue, bookings, and margins in one place, current, without asking anyone to pull them. I built the executive view that every CXO now uses to track the business.

**Lead allocation and seller configuration.**
Leads were being distributed by hand, which does not scale and is hard to audit. I built an allocation system with per-seller capacity, a configuration surface team leads manage themselves, and a ticketing flow so every change is logged and reversible.

**Incentive computation.**
Sales incentives were being worked out in spreadsheets, which is slow and easy to get wrong when the rules change mid-quarter. I built the logic that computes incentives from the live booking data under the current slab rules, so payout numbers are reproducible and the rule changes live in one place.

**Tool-adoption analytics.**
We rolled out a new dialer and a messaging tool across the sales team, and I managed the rollout as a program. To know honestly whether the team was using them, I built an adoption dashboard that attributes the gap: where usage is low, how much it would move if it were fixed, and at which team the gap actually sits.

**Funnel performance reporting.**
Different teams were quoting different conversion rates because they were counting the funnel differently. I built one funnel report with a single agreed definition, so every rate on every surface reconciles.

**Data-quality audits.**
Some of the most useful work is invisible. I built audits that catch silent problems before they reach a report, like deals back-entered against the wrong date, or two systems that quietly disagree by exactly five and a half hours.

## What I work with

- **Data:** PostgreSQL, BigQuery, MongoDB
- **Analysis and BI:** Python (pandas), Metabase
- **Building and shipping:** Next.js, Python services, deployed on Vercel
- **The unglamorous glue:** SQL and documentation

## Reach me

- LinkedIn: https://www.linkedin.com/in/agnidh-ghosh-a439551b7/
- Email: agnidh@gmail.com
