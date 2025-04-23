# Reflection

This section highlights our group’s collective experience during the software maintenance simulation — what went well, what didn’t, and what we learned through the process. As the Tier 3 engineer and team leader, I also include my personal perspective on coordinating the workflow.

---

## What Went Well

- **Role clarity and tier-based assignment** helped us focus. Everyone knew their responsibilities, which reduced overlap and confusion.
- Our **escalation decisions were timely and accurate**. We avoided dragging issues within the wrong tier and ensured critical problems reached the right person quickly.
- We adapted to problems dynamically, especially those that seemed simple at first but revealed deeper issues (e.g., Ticket 2 and Ticket 8).
- Communication was open. Everyone contributed and voiced uncertainties when needed — which helped us maintain momentum.

---

## What Didn’t Go So Well

- **Ticket 3 was escalated too late.** Tier 1 assumed it was a surface-level error, but it required backend routing verification. A faster escalation would have saved us time.
- **Prioritization was occasionally unclear**, especially when multiple medium-priority issues came up. Without an automated board or shared visual dashboard, we had to manually re-align priorities during team check-ins.
- While I took the lead as expected, there were moments where **task delegation could have been more structured** — clearer handoffs might have saved back-and-forth communication.

---

## A Moment of Team Misalignment

One particular challenge we faced was during the mobile payment issue (Ticket 2). Initially, it was classified as a configuration error by Tier 2, but it quickly became apparent that it involved external integration with a payment gateway. It took some time before it was escalated to me at Tier 3, which caused delays in resolution.

The lesson here was that **it's better to escalate early if there’s uncertainty, rather than risk misdiagnosis**.

---

## If AI Tools Had Been Available…

Had we been allowed to use AI tools, we could have:
- Automated **log analysis and crash diagnostics** (especially for Android compatibility issues).
- Used AI to **suggest dependency patching plans** and detect CVEs early.
- Generated summaries and resolutions more efficiently, helping us move faster with documentation.

---

## Leadership and Coordination

As the team leader, I made sure to:
- Start each session with a check-in and clear plan.
- Assign tasks based on real-world tier logic.
- Step in where deep technical intervention was needed.
- Keep the flow of communication active across all tiers.

This experience solidified the importance of leadership that balances **technical depth with process clarity**. It taught me that managing people during maintenance is just as important as managing the system itself.

---

In the end, the simulation gave us a realistic, hands-on feel of how structured support teams operate — and where human communication, critical thinking, and decision-making truly matter.
