#  Coaching Module: The SM in the Daily Stand-up (DSU)

Effective Daily Stand-ups (DSU) are the heartbeat of a sprint. This module outlines how a Scrum Master transitions from a passive observer to a strategic facilitator.

---

## 1. The Mindset Shift: Facilitator vs. Secretary
The most common mistake an SM makes is acting as a **"Secretary"** (taking notes and updating Jira) or a **"Boss"** (asking "What did you do yesterday?").

* **The Goal:** The DSU is for the **Developers**, not the SM. 
* **The SM's Role:** Ensure the meeting happens, stays within the timebox, and identifies blockers.

## 2. The SM's "Active Listening" Strategy
During the 15-minute session, the SM should be listening for **"Invisible Blockers"**:

* *"I'm almost done":* If a dev says this three days in a row, they are stuck.
* *"I'm waiting for a reply":* This is a dependency.
* *"I'm just fixing a few bugs":* This might be **Scope Creep** or **Gold Plating**.

---

##  The "Effective DSU" Checklist for Scrum Masters

###  Before the DSU (Preparation)
- [ ] **Metric Check:** Check the CI/CD Pipeline (e.g., Bitrise/GitHub Actions). Is the build red? Is it slow?
- [ ] **Board Health:** Scan the Jira/Azure board. Are there tickets with no updates for 2 days?
- [ ] **Environmental Prep:** Ensure the link is active (remote) or the physical board is ready (office).

###  During the DSU (Facilitation)
- [ ] **The "15-Minute" Rule:** Start exactly on time. End on time.
- [ ] **Walk the Board:** Focus on the tickets (**Right to Left**). Ask: *"What do we need to do to move this 'In Progress' ticket to 'Done'?"*
- [ ] **Blocker Capture:** When a blocker is raised, do not solve it now. Note it down for the "Meet-After."
- [ ] **Dependency Watch:** In a SAFe context, specifically ask: *"Is this blocking another team (Backend/Platform), or are they blocking us?"*

### After the DSU (Execution)
- [ ] **The "Meet-After":** Facilitate a 5–10 minute deep dive only for the people needed to solve the specific blocker.
- [ ] **Escalation:** If a blocker is external (e.g., Identity Provider is down), immediately prepare for the Scrum of Scrums (SoS).
- [ ] **Update Radiators:** If a risk was identified, update the Program Board or Risk Register.

---

##  Advanced Techniques for Scaled Projects (Nexus/SAFe)

### A. The "Nexus Daily Scrum" Focus
If you are in a Nexus, your DSU must prioritize **Integration**.
> **Coaching Tip:** Ask the team: *"Did anyone commit code yesterday that might break the React Native bridge for the iOS sub-team?"*

### B. The "SLA Enforcement"
If the team is blocked by the Backend, coach them on the SLA/Swagger contract.
> **Coaching Tip:** *"Since the API isn't ready yet per our agreement, let's switch to the Mockoon mock server so we don't lose today's development time."*

---

##  Sample Script for the SM

| Situation | What the SM should say |
| :--- | :--- |
| **Problem Solving** | "This sounds like a technical deep dive. Let's park this for the 'Meet-After' so we can respect everyone's time." |
| **Stalled Ticket** | "I see this ticket has been in 'Testing' for 3 days. What is the bottleneck, and how can we get it across the line?" |
| **External Blocker** | "I'll take the lead on contacting the DevOps team about the pipeline delay. I'll have an update for you by 11:00 AM." |

---
