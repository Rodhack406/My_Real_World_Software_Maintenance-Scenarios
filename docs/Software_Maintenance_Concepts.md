# Understanding Software Maintenance

## What Is Software Maintenance?

Software maintenance refers to the process of modifying and updating software applications after delivery to correct faults, improve performance, or adapt the product to a changed environment. It ensures that software continues to meet user needs and remains reliable and secure over time.

## Types of Software Maintenance

1. ### Corrective Maintenance
   - Fixing bugs and defects discovered after deployment.
   - Example: Patching a broken login button or crashing app.

2. ### Adaptive Maintenance
   - Updating software to keep up with changing environments or platforms.
   - Example: Ensuring compatibility with Android 12 or new web browsers.

3. ### Perfective Maintenance
   - Enhancing features or improving code structure without changing core functionality.
   - Example: Refactoring messy code or optimizing load times.

4. ### Preventive Maintenance
   - Making changes to prevent future problems.
   - Example: Updating a dependency to prevent security vulnerabilities (CVE fixes).


## Why Is It Important?

- User Experience: Bugs or slow systems frustrate users.
- Security: Unpatched software is a major security risk.
- Scalability: Well-maintained systems scale more easily.
- Reputation: Reliability builds user and stakeholder trust.


## The Tiered Support Model

In real-world maintenance, problems are typically assigned to support tiers based on their complexity and urgency:
- Tier 1: Handles simple or routine issues (FAQs, UI glitches).
- Tier 2: Handles more complex problems (configuration, known issues).
- Tier 3: Handles deep technical issues requiring code knowledge or developer input.
Each tier has the responsibility to either resolve the problem or escalate it to the next level.


## Triage and Prioritization

### Triage is the act of evaluating and prioritizing incoming issues. Key factors include:

- Severity: How much impact does it have on users?
- Frequency: How often does it occur?
- Reproducibility: Can it be reliably replicated?
- Scope: Is it isolated or system-wide?
Proper triage ensures the most urgent issues get addressed first and helps avoid burnout.


## Communication in Maintenance

Clear, timely communication between support tiers, developers, and stakeholders is crucial. It includes:
- Reporting issues
- Escalation pathways
- Documentation of resolution steps
- Status updates
Lack of communication often leads to delays, duplicated effort, or mismanagement of critical issues.


## Tools That Assist Maintenance

- Monitoring tools (e.g., Sentry, Datadog) — for error tracking
- Version control (e.g., Git) — for tracking changes
- CI/CD pipelines — for automated testing and deployment
- Issue trackers (e.g., GitHub Issues, Jira) — for managing tickets


## Key Concepts Covered in This Repository

- Security patching (CVE report triage)
- Dependency management (Spring Boot versioning)
- Feature conflicts (QA and release mismanagement)
- Bug escalation
- Cross-tier collaboration
- Response time estimation
- Reflective learning and documentation


## Who Is This For?

This guide is helpful for:
- Students learning about real-world software support
- Junior developers looking to improve system reliability skills
- Teams building internal maintenance processes

@author: _Moses Kaluba
