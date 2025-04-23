## How the Simulation Was Conducted

This document provides a detailed breakdown of how our team conducted the software maintenance simulation lab.


### Overview of the Lab

The lab was a simulation of real-world software maintenance practices. As a Team we were expected to:

- Form a structured team with Tier 1, Tier 2, and Tier 3 support roles.
- Review a set of maintenance tickets representing real system problems.
- Prioritize and assign these tickets based on severity and complexity.
- Resolve the issues or escalate them through the appropriate support tiers.
- Document resolution logs and reflect on the communication, process, and collaboration.

---

## Team Composition

I led a team of three members, each assigned a different tier of support:

- **Tier 1 – Nephas Knago**: First point of contact for minor, easily reproducible issues.
- **Tier 2 – Rayford Kangoji**: Responsible for handling intermediate issues involving configuration, data processing, or logic.
- **Tier 3 – Moses Kaluba (myself)**: Acted as the lead engineer handling critical and deep technical issues. I also served as the **Team Leader**, coordinating task distribution and escalation paths.

---

## List of Tickets

| Ticket ID | Description                                                                                      | Severity |
|-----------|--------------------------------------------------------------------------------------------------|----------|
| 1         | Admin users cannot log in, but regular users can.                                                | High     |
| 2         | Errors when completing mobile payments.                                                          | Critical |
| 3         | Contact Us button on the homepage redirects to a 404 page.                                       | Low      |
| 4         | Integration API starts rejecting requests after 200 calls/hour.                                  | Medium   |
| 5         | Reporting dashboard takes 10–15 seconds to load each time.                                       | Medium   |
| 6         | Alert triggered for downtime at 2 AM, but no actual outage was observed.                         | Low      |
| 7         | App crashes instantly on Android 7 and below.                                                    | High     |
| 8         | CVE report suggests a vulnerable library in use (Spring Boot 2.4.1).                             | Medium   |
| 9         | Two separate features released on the same day overwrite each other’s changes in production.     | Critical |

---

##  Ticket Assignments and Rationale

### Ticket 3 – “Contact Us button redirects to 404”
- **Assigned to:** Nephas Knago (Tier 1)
- **Reason:** This was a UI-level issue likely caused by a misconfigured route or broken link. Tier 1 handles common frontend errors and page behaviors.



### Ticket 6 – “False alert triggered at 2 AM”
- **Assigned to:** Nephas Knago (Tier 1)
- **Reason:** Monitoring-related false positives typically fall within Tier 1's responsibilities, especially if no real user impact is observed.



### Ticket 4 – “API rejects requests after 200 calls/hour”
- **Assigned to:** Rayford Kangoji (Tier 2)
- **Reason:** This issue hinted at either a rate limiting misconfiguration or throttling logic, which falls into Tier 2's scope of work (config-level analysis).



### Ticket 5 – “Dashboard takes 10–15 seconds to load”
- **Assigned to:** Rayford Kangoji (Tier 2)
- **Reason:** Performance degradation typically requires data analysis and optimization strategies. Tier 2 was suitable unless code-level refactoring was required.



### Ticket 2 – “Errors with mobile payment processing”
- **Initially Assigned to:** Rayford Kangoji (Tier 2)  
- **Escalated to:** Moses Kaluba (Tier 3)
- **Reason:** It was first treated as a config issue, but upon closer inspection it involved integration with a third-party payment gateway. I stepped in from Tier 3 to assist due to the need for developer-level knowledge and error tracing.



### Ticket 1 – “Admin login fails, regular login works”
- **Assigned to:** Moses Kaluba (Tier 3)
- **Reason:** A login bug affecting user roles required backend analysis and access control verification. This was clearly in Tier 3's domain.



### Ticket 7 – “App crashes on Android 7 and below”
- **Assigned to:** Moses Kaluba (Tier 3)
- **Reason:** Device-level crashes and OS-specific bugs usually require deep debugging and dependency checks, appropriate for Tier 3 support.



### Ticket 8 – “CVE report – Spring Boot 2.4.1 vulnerability”
- **Initially Assigned to:** Rayford Kangoji (Tier 2)  
- **Escalated to:** Moses Kaluba (Tier 3)
- **Reason:** Although dependency updates start as a Tier 2 task (via audits), this required validation at the code level and planning around backward compatibility — so I took over.



### Ticket 9 – “Feature overwrite in production”
- **Assigned to:** Moses Kaluba (Tier 3)
- **Reason:** This was a major coordination failure involving feature merges and production deployment. As the team lead and Tier 3 engineer, I addressed the root cause and proposed a QA and CI/CD fix.



## Summary

This lab was structured to simulate the exact dynamics found in real software teams. We used tiered assignment to mimic professional escalation structures and ensured that each ticket was triaged thoughtfully. I personally handled the most technically complex issues while overseeing team coordination and decision-making as the lead.

Our assignments were realistic and rooted in how production-level incidents are resolved across support and engineering teams.

