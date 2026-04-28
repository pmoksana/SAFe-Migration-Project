---
layout: default
title: Team-to-Team OLA
---


# The Social Contract: Working Agreements for Scaled Mobile Teams

A **Working Agreement (WA)** is a social contract that defines how teams interact to prevent friction. In SAFe, these are often referred to as **Team-to-Team OLA** (Operating Level Agreements).

Below are specific working agreements tailored to the unique challenges of **Mobile Development** and **React Native Migrations**.

---

## 1. The "Definition of Ready" (DoR) for Dependencies
To eliminate the "waiting on the API" bottleneck, create a hard contract between Mobile and Backend (BE) teams.

* **The Agreement:** *"The BE team must provide a Swagger/OpenAPI specification and a Mock Endpoint at least 3 days before the Mobile team starts the Sprint."*
* **Why it works:** React Native devs can build UI and logic against "mock" data without being blocked by backend logic.
* **The SM Role:** If the BE team fails this, raise it in the **Scrum of Scrums** immediately as a "Blocker for the next Sprint."
---

## 2. Shared "Definition of Done" (DoD) for Migration
Legacy platforms often introduce "new" bugs during a migration.

* **The Agreement:** *"A feature is not 'Done' until it passes automated tests on both physical iOS and Android devices, and the 'Legacy' feature toggle is verified."*
* **Why it works:** It kills the *"It works on my iPhone"* syndrome common in hybrid development.

---
## 3. The "Cross-Platform Sync" Agreement
When a team is split into iOS and Android sub-teams, they often drift apart in their React Native implementation.

* **The Agreement:** *"Any new Bridge Module (native hardware integration) must be peer-reviewed by at least one member from the 'opposite' platform."*
* **Why it works:** It prevents "Platform Silos" and ensures the codebase doesn't become a black box to half the team.

----
## 4. The "Communication Protocol" (The 4-Hour Rule)
In scaled environments, waiting for the next DSU to report a blocker results in massive waste.

* **The Agreement:** *"If a cross-team dependency blocks progress for more than 4 hours, it must be escalated via the dedicated `#SOS-Blocker` channel immediately."*
* **Why it works:** It empowers the Scrum Master to coordinate with other SMs in real-time rather than waiting for formal meetings.

---
## 5. The "Refinement Handshake"
* **The Agreement:** *"Any ticket involving a shared React Native component must have a 'Technical Lead Sync' before it is pulled into a Sprint."*
* **Why it works:** Ensures leads agree on architecture *before* coding starts, preventing costly mid-sprint re-work.

---

## 🛠️ How to Implement: The Scrum Master’s Strategy

If you are struggling with **Post-Migration Support** (juggling old vs. new platforms), propose a **Hotfix Agreement**:

> **Example Agreement:** *"High-priority bugs in the Legacy platform will be handled by a Rotating Support Pair (1 iOS, 1 Android) to ensure the rest of the team remains focused on React Native migration goals."*

### How to "Coach" these agreements into existence:

1.  **Identify the Pain:** Use data in your Retrospective. *"We spent 30 hours this sprint waiting for the API team."*
2.  **Propose the Solution:** *"What if we asked them to agree to a 'Mock API' contract?"*
3.  **Formalize:** Document the agreement in your team’