
# Navigating Scaled Agile: A Guide to Mobile Migration
> **Frameworks in Focus:** SAFe & Nexus  
> **The Mission:** Transitioning from Native (Swift/Java) to React Native at Scale.

---

## 1. Coordinating Sprints, Events, and Dependencies
**The Goal:** Facilitating seamless alignment across distributed teams.

###  The Technique
*   **SAFe (Scrum of Scrums):** Facilitating bi-weekly or daily SoS meetings to resolve cross-team dependencies.
*   **Nexus (Nexus Daily Scrum):** Team representatives meet with the Nexus Integration Team to ensure iOS/Android sub-teams aren't blocking the **Integrated Increment.**

###  Real-World Challenges
> [!IMPORTANT]
> **Challenge I: The BE Bottleneck**  
> *Problem:* Backend APIs are delayed while Mobile teams are ready.  
> **Action:** Negotiated **Mock API Contracts**. During the SoS, raised a "Risk." Negotiated a "Mock" contract so devs could continue building in React Native while the BE caught up.

> [!WARNING]
> **Challenge II: The Platform Split**  
> *Problem:* iOS and Android teams are out of sync on features.  
> **Action:** **Synchronized Sprint Starts**. Enforced a shared Sprint Goal. Used Nexus Integration concepts to ensure both platforms merge code into a single **Release Candidate** by the end of the sprint.

---

## 2. Removing Impediments & Barriers
At scale, impediments shift from local issues to systemic "Platform Blockers."

### 🛡 The Scrum Master as a Shield
*   **External Dependencies:** The legacy "Identity Provider" was unstable, stalling the React Native migration.
    *   **Action:** Established a **Service Level Agreement (SLA)** with the Legacy Team manager to prioritize critical bug fixes.
*   **Hardware Shortages:** The iOS team lacked powerful MacBooks to run heavy React Native builds.
    *   **Action:** Escalated to the **RTE (Release Train Engineer)** in SAFe, demonstrating the **Cost of Delay** (e.g., "We are losing 10 hours of dev time per week").

---

## 3. Capacity Planning & Backlog Management
Migration creates a "Learning Curve" that makes capacity unpredictable.

###  Planning Strategy
*   **SAFe PI Planning:** Looking 8–12 weeks ahead to anticipate the transition.
*   **Nexus Refinement:** Identifying if a Product Backlog Item (PBI) affects both platforms simultaneously.

###  Solutions
> [!TIP]
> **The "Learning Tax"**  
> *Challenge:* Developers are slower when learning TypeScript/React Native.  
> **Action:** Facilitated **Capacity Buffers**. Coached the PO to plan only 60% of historical velocity to allow for research **Spikes**.

> [!NOTE]
> **Post-Migration Support**  
> *Challenge:* High bug counts after going live on the new stack.  
> **Action:** Implemented a **Split Capacity Model** (70% New Features / 30% Platform Stabilization) to handle tech debt.

---

## 4. Coaching Self-Management & Cross-Functionality
**Goal:** Transition from "iOS/Android Devs" to **"Mobile Engineers."**

###  Breaking Silos
*   **Problem:** iOS devs refusing to review Android code ("Platform Pride").
*   **Action:** Facilitated **Pair Programming** on React Native "Bridge" modules. Explained that since 80% of the code is shared, silos are a blocker to the **Definition of Done (DoD)**.

###  Definition of Done (DoD)
*   **Challenge:** Inconsistency in "Done" leads to broken releases (e.g., "Works on iPhone but not Android").
*   **Action:** Facilitated a workshop to create a **Nexus-level DoD**. A ticket is only "Done" when the React Native build passes on **both** physical test devices.

---

## 5. Stakeholder Collaboration & Metrics
Stakeholders need data-driven confidence during a complex tech migration.

###  Key Metrics
*   **System Demo (SAFe):** Bi-weekly demos of the integrated app to prove progress.
*   **Migration Burn-up Chart:** Instead of just showing Velocity, we track **"Native Features Retired" vs. "React Native Features Live."**

###  Managing Expectations
*   **Challenge:** Clients demanding new features *and* migration simultaneously.
*   **Action:** Facilitated a **Prioritization Matrix**. Visualized the **Critical Path**, proving that the "New Checkout" cannot exist until the "React Native Core" is stable.

---
*Created for the Engineering Blog — Focused on Agile Excellence.*