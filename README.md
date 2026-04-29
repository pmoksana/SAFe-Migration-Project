
## Содержание проекта

* [ Daily Stand-up](Daily-Stand-up)
* [ SAFe Guide](SAFe-Guide)
* [ Scaled Events Playbook](Scaled-Events-Playbook)
* [ Scrum of Scrums](Scrum-of-Scrum)
* [ Team-to-Team OLA](Team-to-Team-OLA)
* [ Metricks](Metricks)
* [Release Management Sync](Release-Management-Sync)
* [SoS Devops Challenge] (SoS-Devops-Challenge)

### SCrum master Role 

I manage my team’s calendar to synchronized all ecosystem of project ensuring that multiple teams are working together toward a single integrated goal.
###  Scaling & Coordination (SAFe / Nexus)
Facilitate Scaled Events: Dayly stand up  I facilitate my team’s 15-minute sync, I specifically listening for "External Dependencies" (e.g., "The API is down").
After I attend the SoS. I represent my team’s progress and blockers to the other Scrum Masters and the Release Train Engineer (RTE)my goal is to  to synchronize the "Release Train" and manage cross-team dependencies.

*  "I used the Scrum of Scrums to resolve a backend dependency, and ensured the React Native migration stayed on schedule."
*  Facilitate a tech-debt task to fix or remove impediments for example the "flaky" test. [SoS Devops Challenge](SoS-Devops-Challenge)


Release Train Alignment: Ensure the team hits Code Freeze dates and stays aligned with the synchronized 2-week sprint cadence of the wider organization.
Continuous Improvement: I Lead retrospectives in case of systemic issues affecting the entire Agile Release Train (ART).

### Coordinate the "Release Train" Schedule
I align my team to a pre-set Release Calendar.

The Cut-off Date: I check the "Code Freeze" date. If my Sprint ends on Wednesday, but the Release Train leaves on Monday, my team work must be "Done-Done" and merged by Monday morning.

>>Sync Meetings: I attend the Release Management Sync (usually once a week). [Release Management Sync](Release-Management-Sync)

So In this meeting, the Release Train Engineer (RTE) and Release Managers are looking for one thing: Confidence. They want to know if your team's code is safe to ship to thousands of users on the App Store and Google Play.

Your Role: You report the status of the React Native migration features. "Feature A is 100% and passed QA; Feature B is at risk due to a Google Play library conflict."

Submission Window: You coordinate the "Binary Upload." For example, the Release Team might require the build to be in App Store Connect by Thursday to allow for a 48-hour "internal smoke test" before hitting "Submit for Review."


Dependency Management: Identify and visualize "Red String" dependencies during PI Planning and cross-team refinement sessions.

Coordinate the "Integrated Increment": Work  Integration Team CICD Devops to ensure iOS and Android sub-teams merge code into a single, testable React Native build.

### Retrospectives: Solving Systemic Issues
A retro fixes we discudd "how the organization works."

The Team Retro: You help the team identify internal friction (e.g., "Our iOS/Android pairing isn't working").

The Inspect & Adapt (I&A) / I take the "Systemic Issues" (e.g., "The CI/CD pipeline is too slow for all 3 teams") to the Program-level retrospective.

Action Item Coordination: If a change requires another team to act (like the Backend team changing their testing process), you work with the other Scrum Master to ensure that action item actually gets implemented.






### Technical Facilitation (The "Bridge" Role)
Enforce "Contract-First" Development: Facilitate Working Agreements between Mobile and Backend teams (e.g., ensuring Swagger/OpenAPI specs are delivered 3 days before a sprint).

Monitor Flow Metrics: Proactively track CI/CD pipeline duration (using tools like Bitrise/GitHub Actions) to identify bottlenecks and coordinate with DevOps for optimization.

Remove Systemic Impediments: Manage Service Level Agreements (SLAs) with external providers (like Identity Providers) to ensure environment stability.

Shield the Team: Act as a filter for technical distractions, allowing devs to focus on the React Native migration during the high-intensity "Learning Phase."

###  Product & Stakeholder Partnership
Refine the "Definition of Ready": Assist the PO in ensuring backlog items meet the DoR, including validated API mocks and UX designs, before sprint commitment.

Phased Release Coordination: Partner with Release Management to oversee staged rollouts (1% → 100%) and monitor crash reporting (Sentry/Crashlytics) for "Go/No-Go" decisions.

Stakeholder Transparency: Facilitate System Demos to showcase high-value increments to business owners, focusing on the ROI of the new technology stack.

Capacity Planning: Coordinate with the PO to balance new feature delivery with Post-Migration Support and technical debt cleanup.

###  Team Coaching & Culture
Drive Cross-Functionality: Coach developers to move from "Platform Silos" (iOS vs. Android) to Feature Ownership, encouraging pair programming within the React Native codebase.

Uphold Quality Standards: Facilitate the creation of a Nexus-level Definition of Done, requiring features to be verified on both platforms before being marked complete.

Continuous Improvement: Lead retrospectives that address not just team dynamics, but systemic issues affecting the entire Agile Release Train (ART).

Empower Self-Management: Foster an environment where the team can pivot to "Mocked" development or technical debt tasks independently when blocked by external factors.
















# Navigating Scaled Agile: A Guide to Mobile Migration
> **Frameworks in Focus:** SAFe & Nexus  
> **The Mission:** Transitioning from Native (Swift/Java) to React Native at Scale.

---
SM Role 
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