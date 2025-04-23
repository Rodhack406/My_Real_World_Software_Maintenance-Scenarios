# Escalation Strategy

In any real-world maintenance setup, proper escalation is essential for resolving complex issues efficiently. During our simulation, we adopted a structured approach to escalating tickets based on severity, complexity, and required expertise.

As the team leader and Tier 3 engineer, I worked closely with Rayford (Tier 2) and Nephas (Tier 1) to determine when issues should remain within a tier or be passed up the chain.

---

## When and Why We Escalated

### Our Escalation Criteria:
- **Technical complexity** beyond the current tier's capacity
- **Blocked resolution** after initial attempts
- **Issues involving external systems**, APIs, or security implications
- **Need for code-level debugging** or access beyond Tier 1 or 2

---

## Real Examples from the Simulation

### Ticket 2 – *Mobile Payment Errors*
- **Escalated from Tier 2 to Tier 3**
- Initially seemed like a configuration issue, but after failing to resolve it, Rayford (Tier 2) escalated the problem. I discovered it involved third-party gateway behavior that required deeper debugging — typical Tier 3 responsibility.

---

### Ticket 3 – *Contact Us Button Leads to 404*
- **Escalated from Tier 1 to Tier 2**
- Nephas identified the broken link, but routing verification and deployment traceability exceeded Tier 1’s scope. Rayford took over and traced the issue to an incorrect route mapping.

---

### Ticket 5 – *Dashboard Performance Delay*
- **Escalated from Tier 2 to Tier 3**
- Rayford noticed load delays but lacked access to optimize the data-fetching logic or restructure backend queries. I stepped in to review and optimize the performance at code level.

---

### Ticket 8 – *CVE Report for Spring Boot 2.4.1*
- **Escalated from Tier 2 to Tier 3**
- While Rayford conducted the initial dependency audit, I took over to validate the patch impact, ensure backward compatibility, and plan remediation steps — typical of Tier 3’s role in security-related maintenance.

---

## Key Takeaways

- We avoided unnecessary escalations by letting each tier investigate first.
- Escalation wasn’t seen as failure — but as **strategic collaboration**.
- We always included communication notes with escalations so the next tier could pick up without confusion.
- As team lead, I ensured escalations were handled smoothly and without delay, preserving workflow clarity and issue momentum.

---

This strategy helped our team simulate a real engineering support environment and reinforced the importance of assigning the **right task to the right tier**, at the right time.
