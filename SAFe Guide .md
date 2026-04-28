
---
layout: default
title: SAFe Migration Project
---

## 1. Coordinating Sprints, Events, and Dependencies
**The Goal:** Facilitating seamless alignment across distributed teams.

###  The Technique
* **SAFe (Scrum of Scrums):** Scrum Masters (SM) attend bi-weekly or daily SoS meetings to resolve cross-team dependencies.
* **Nexus (Nexus Daily Scrum):** Team representatives meet with the Nexus Integration Team to ensure iOS/Android sub-teams aren't blocking the **Integrated Increment.**

###  Real-World Challenges
| Challenge | Action Taken |
| :--- | :--- |
| **The BE Bottleneck:** Backend APIs are delayed while Mobile teams are ready. | **Mock API Contracts:** Negotiated a "Mock" contract so developers could continue building in React Native while the BE caught up. |
| **The Platform Split:** iOS and Android teams are out of sync on features. | **Synchronized Sprint Starts:** Enforced a shared Sprint Goal and used Nexus Integration concepts to merge code into a single **Release Candidate.** |

Challenge I: The BE Bottleneck. SM iOS/Android teams are ready, but the Backend (BE) API is delayed.

Action: During the SoS, SM raise a "Risk" or "Blocker." SM negotiate a "Mock API" contract so mobile devs can continue working in React Native while BE catches up.

Challenge II: The Platform Split. iOS and Android sub-teams are out of sync on a feature.

Action: SM implement a Synchronized Sprint Start. Even if they are sub-teams, they must share the same Sprint Goal. SM use the Nexus Integration Sprint concept to ensure both platforms merge code into a single "Release Candidate" by the end of the sprint.


---


## 2. Removing Impediments & Barriers
At scale, impediments shift from "the internet is down" to "Team B didn't finish the SDK."

* **Scrum of Scrums:** Focused on cross-team blockers.
* **Nexus:** Focused on integration issues (e.g., React Native bridge failing on one OS).

> [!IMPORTANT]
> **Case Study: The Legacy Platform Shield**
> **Problem:** The old "Identity Provider" was unstable, stalling the React Native migration.
> **Action:** Acted as a shield by establishing a **Service Level Agreement (SLA)** with the Legacy Team manager to prioritize critical bug fixes.

Challenge: External Dependencies (The Legacy Platform). SM team is migrating to React Native, but the old platform’s "Identity Provider" (login system) is unstable.

Action: SM act as a Shield. SM meet with the Legacy Team’s manager to establish a "Service Level Agreement" (SLA) for bug fixes so SM React Native migration isn't stalled by old tech.

Challenge: Hardware Shortages. The iOS team doesn't have the latest MacBooks to run the heavy React Native build processes.

Action: SM escalate this to the Release Train Engineer (RTE) in SAFe, demonstrating the cost of delay (e.g., "We are losing 10 hours of dev time per week").
---


## 3. Capacity Planning & Backlog Management
Migration creates a "Learning Curve" that makes capacity unpredictable.

###  Planning Strategy
* **SAFe PI Planning:** Looking 8–12 weeks ahead.
* **Nexus Refinement:** Identifying if a Product Backlog Item (PBI) affects both platforms simultaneously.

###  Solutions
* **The "Learning Tax":** Developers are slower when learning TypeScript. 
    * *Action:* Facilitated **Capacity Buffers**, planning only 60% of historical velocity to allow for research "Spikes."
* **Post-Migration Support:** High bug counts after going live.
    * *Action:* Implemented a **Split Capacity Model** (70% New Features / 30% Platform Stabilization).


Challenge: The "Learning Tax" in Migration. Developers are slower because they are learning TypeScript/React Native.

Action: SM facilitate Capacity Buffers. SM coach the PO to only plan 60% of the team's historical native velocity for the first two sprints of the migration to allow for "Spikes" (research tasks).

Challenge: Post-Migration Support. The new platform is live, but bugs are high.

Action: SM implement a "Split Capacity" model. 70% of capacity goes to new React Native features; 30% is reserved for "Platform Stabilization" to handle the tech debt of the old platform technology.
---


## 4. Coaching Self-Management & Cross-Functionality
**Goal:** Transition from "iOS/Android Devs" to **"Mobile Engineers."**

###  Breaking Silos
* **Problem:** iOS devs refusing to review Android code.
* **Action:** Facilitated **Pair Programming** on React Native "Bridge" modules. Explained that since 80% of the code is shared, "Platform Pride" is a blocker to the Definition of Done (DoD).

###  Definition of Done (DoD)
Inconsistency in "Done" leads to broken releases. We implemented a **Nexus-level DoD**: A ticket is only "Done" when the React Native build passes on *both* physical test devices.

Challenge: Siloed Sub-teams. The iOS devs refuse to review Android code.

Action: SM facilitate Pair Programming sessions. SM pair an iOS dev with an Android dev on a React Native "Bridge" module. SM explain that in React Native, 80% of the code is shared, so "Platform Pride" is a blocker to "Done."

Challenge: Definition of Done (DoD) Inconsistency. The iOS sub-team thinks "Done" means "Works on iPhone," while the business expects "Works on both."

Action: SM facilitate a workshop to create a Nexus-level DoD. A ticket isn't "Done" until the React Native build passes on both physical test devices.
---

## 5. Stakeholder Collaboration & Metrics
Stakeholders need data-driven confidence during a migration.

###  Key Metrics
* **System Demo (SAFe):** Bi-weekly demos of the integrated app.
* **Migration Burn-up Chart:** Instead of just showing Velocity, we track **"Native Features Retired" vs. "React Native Features Live."**

###  Managing Expectations
When clients demand new features *and* migration simultaneously, use a **Prioritization Matrix**. This visualizes the **Critical Path**, proving that the "New Checkout" cannot exist until the "React Native Core" is stable.

---
*Created for the Engineering Blog — Focused on Agile Excellence.*
Challenge: Reporting Progress during Migration. Stakeholders ask, "Why is velocity down?"

Action: SM implement a Migration Burn-up Chart. It shows the "Native Features Retired" vs. "React Native Features Live." This shifts the focus from "Story Points" to "Business Value Delivered on the New Tech."

Challenge: Managing Client Expectations. The client wants all new features and the migration finished at the same time.

Action: SM facilitate a Prioritization Matrix with the PO and Client. SM show them the "Critical Path" (e.g., "We can't build the new Checkout until the React Native Core is stable").

# Navigating Scaled Agile: A Guide to Mobile Migration
> **Frameworks in Focus:** SAFe & Nexus  
> **The Mission:** Transitioning from Native (Swift/Java) to React Native at Scale.

 ---
 ### 📋 Summary Table: Scrum Master Strategic Actions

| Responsibility | SAFe / Nexus Action | React Native Migration Example |
| :--- | :--- | :--- |
| **Impediments** | **Nexus Integration Team** | Resolving a library conflict that breaks the Android build while the iOS build remains stable. |
| **Capacity** | **PI Planning / Buffers** | Accounting for a **20% "Velocity Drop"** during the first 3 weeks as the team adopts the React Native stack. |
| **Coaching** | **Cross-functionality** | Mentoring developers to transition from "Platform Specialists" to "Feature Owners" who manage the shared codebase. |
| **Refinement** | **Multi-team Refinement** | Ensuring Backend (BE) developers align on the specific JSON structures required for new React Native API calls. |

---

