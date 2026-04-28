---
layout: default
title: Scrum Master Scaled Events Playbook
---

#  Scrum Master Scaled Events Playbook
> **Environment:** SAFe / Nexus  
> **Focus:** Mobile (iOS/Android) & React Native Migration Projects

This document outlines the specific roles, coaching questions, and checklists for a Scrum Master operating at scale. Use this as a guide to maintain quality and alignment across distributed mobile teams.

---

## 1. Sprint Planning
**Goal:** Align on the Sprint Goal and commit to a plan that accounts for cross-platform dependencies.

| SM Role | Key Questions to Ask |
| :--- | :--- |
| **The Negotiator** | "Does this story meet our Definition of Ready (e.g., is the Swagger spec available)?" |
| **Capacity Planner** | "Are we accounting for the 20% 'Learning Tax' for the new React Native modules?" |
| **Dependency Mapper** | "Which stories are blocked by the Backend or Platform teams this sprint?" |

### ✅ Checklist
- [ ] Capacity is calculated minus vacations, public holidays, and "IP" time.
- [ ] Every Story has clear Acceptance Criteria.
- [ ] A Sprint Goal is defined that describes the value (e.g., "Enable User Login via React Native").
- [ ] Dependencies are flagged in Jira/Azure DevOps and communicated to other Scrum Masters.

---

## 2. Daily Stand-up (DSU)
**Goal:** Synchronize the team and identify blockers to the Sprint Goal.

| SM Role | Key Questions to Ask |
| :--- | :--- |
| **Guardian of Flow** | "What is stopping us from moving this ticket to 'Done' today?" |
| **Technical Watchman** | "I see the Bitrise build failed for Android; do we have an owner for that?" |
| **Facilitator** | "This is a deep technical topic—can we move this to the Meet-After?" |

### ✅ Checklist
- [ ] Started and ended in 15 minutes.
- [ ] Board was "walked" from Right to Left (Focus on finishing).
- [ ] Blockers were identified and visualized (Red tags/stickers).
- [ ] "Meet-After" participants were identified to keep the main meeting concise.

---

## 3. Backlog Refinement
**Goal:** Ensure the Backlog is healthy and stories are "Ready" for future sprints.

| SM Role | Key Questions to Ask |
| :--- | :--- |
| **Technical Facilitator** | "Do we need a Spike to investigate the React Native bridge for this feature?" |
| **Quality Advocate** | "How will we verify this on both physical iOS and Android devices?" |
| **Bridge Builder** | "Is the Backend team aligned on the JSON structure for this API?" |

### ✅ Checklist
- [ ] Top 2 sprints worth of stories are estimated (Story Points).
- [ ] Stories are small enough to be completed within one sprint.
- [ ] Non-functional requirements (Security, Performance) are included in the description.
- [ ] UX/UI designs are attached and reviewed by the developers.

---

## 4. Sprint Review (System Demo)
**Goal:** Demonstrate the "Integrated Increment" to stakeholders and gather feedback.

| SM Role | Key Questions to Ask |
| :--- | :--- |
| **Showrunner** | "Stakeholders, does the performance of this React Native screen meet your expectations?" |
| **Value Reporter** | "We completed 80% of the migration goal; what should we prioritize to finish the rest?" |
| **Feedback Loop** | "Is this feedback a bug, or is it a new requirement for the Backlog?" |

### ✅ Checklist
- [ ] Demo is performed on a **Real Device** (not just a simulator).
- [ ] Integrated code (Mobile + Live Backend) is shown.
- [ ] The "Definition of Done" is confirmed for all demonstrated items.
- [ ] Stakeholder feedback is documented and added to the Backlog.

---

## 5. Sprint Retrospective
**Goal:** Inspect the "How" and create an action plan for team improvement.

| SM Role | Key Questions to Ask |
| :--- | :--- |
| **Coach & Mirror** | "Our cycle time increased by 2 days this sprint—what caused that delay?" |
| **Conflict Resolver** | "How can we better support the pairing between our iOS and Android developers?" |
| **Process Optimizer** | "What is one thing we can change in our Working Agreement to improve our flow?" |

### ✅ Checklist
- [ ] Psychological Safety is established (The Vegas Rule: What happens here, stays here).
- [ ] Data-driven insights (Velocity, Burn-down, Bug counts) are presented.
- [ ] One to Two specific, actionable items are created for the next sprint.
- [ ] Successes are celebrated to maintain team morale.

---

## 6. Scrum of Scrums (SoS) - Scaled Event
**Goal:** Coordinate between multiple teams on the Release Train (Mobile, BE, Platform).

| SM Role | Key Questions to Ask |
| :--- | :--- |
| **Ambassador** | "My team is on track, but we need the Identity Provider (IdP) stable by Tuesday." |
| **Risk Manager** | "Per our SLA, when can we expect the fix for the staging environment?" |
| **Collaborator** | "We found a bug in the shared React Native library; which team can help us peer-review the fix?" |

### ✅ Checklist
- [ ] Blockers requiring external help are escalated to the RTE (Release Train Engineer).
- [ ] The Program Board (Dependencies) is updated.
- [ ] Updates regarding the "Release Train" schedule (Code Freeze, Store Submission) are captured.
- [ ] Information is prepared to be shared back with the team in the next Stand-up.

---

> **Pro-Tip:** In GitHub, the `- [ ]` syntax creates interactive checkboxes. You can check them off directly in the UI if this is part of a GitHub Issue or Task List!