# Issue Resolution Log

## Use of the Issue Resolution Log

As part of our simulation, we used an **Issue Resolution Log** to track every step in our maintenance workflow. This log served as a centralized record of each ticket we received, including its severity, the tier that resolved it, any escalations, time estimates, and notes on communication.

The log is crucial in software maintenance because it provides:
- **Traceability** of decisions and responsibilities
- A **clear history** of how problems were handled
- Insight into **where delays occurred**
- A structured way to **reflect on process efficiency** and improve future handling of issues

In real-world settings, logs like this support accountability, team coordination, and postmortem analysis after incidents. By documenting each action transparently, teams can evaluate what worked well and where changes are needed. It also ensures nothing slips through the cracks — especially during high-pressure maintenance windows.

This table summarizes all maintenance tickets from our software maintenance simulation. It reflects the real-world process of receiving, triaging, escalating, and resolving software issues based on severity and complexity.

We operated as a three-tier support team:
- **Tier 1 – Nephas Knago** handled low-severity, straightforward user-facing issues.
- **Tier 2 – Rayford Kangoji** managed intermediate problems, especially those involving configuration or data handling.
- **Tier 3 – Moses Kaluba (myself)** resolved high-complexity issues requiring code-level intervention and led the overall coordination.

All decisions to escalate were made based on the nature of the issue after initial assessment and team discussion.

---

| Ticket ID | Description                                                                                      | Severity | Tier Resolved | Escalated To | Time (est.) | Communication Notes |
|-----------|--------------------------------------------------------------------------------------------------|----------|----------------|---------------|--------------|----------------------|
| 1         | Admin users cannot log in, but regular users can.                                                | High     | Tier 3         | -             | 35 min       | Assigned directly to Tier 3 by the team lead due to role-based backend logic requirements. |
| 2         | Errors when completing mobile payments.                                                          | Critical | Tier 3         | From Tier 2   | 3 hrs        | Initially investigated by Tier 2; escalated after realizing third-party gateway involvement. |
| 3         | Contact Us button on the homepage redirects to 404 page.                                         | Low      | Tier 2         | From Tier 1   | 1 hr         | Tier 1 identified and passed the issue to Tier 2 for routing and deployment verification. |
| 4         | Integration API starts rejecting requests after 200 calls/hour.                                  | Medium   | Tier 2         | -             | 1 hr 30 min  | Assigned directly to Tier 2 based on API config knowledge. Logs helped narrow it down. |
| 5         | Reporting dashboard takes 10–15 seconds to load each time.                                       | Medium   | Tier 3         | From Tier 2   | 1 hr         | Tier 2 flagged it for code-level optimization after initial performance review. |
| 6         | Alert triggered for downtime at 2 AM, but no actual outage was observed.                         | Low      | Tier 1         | -             | 1 hr 30 min  | Resolved by Tier 1 after determining it was a false positive via system logs. |
| 7         | App crashes instantly on Android 7 and below.                                                    | High     | Tier 3         | -             | 3 hrs        | Reported by users. Assigned to Tier 3 due to OS compatibility and crash analysis. |
| 8         | CVE report suggests a vulnerable library in use (Spring Boot 2.4.1).                             | Medium   | Tier 3         | From Tier 2   | 30 min       | Tier 2 flagged the issue, Tier 3 handled validation and patch planning. |
| 9         | Two separate features released on the same day overwrite each other’s changes in production.     | Critical | Tier 3         | -             | 1 hr         | Assigned to Tier 3 due to merge conflict and production-level deployment issues. |

