

Your Role as Scrum Master in Testing
You are not the person finding bugs; you are the "Quality Advocate" who ensures the environment and process allow for proper testing.

A. During the Sprint (Days 1–8): "Shift-Left" Testing
"Shift-Left" means moving testing to the beginning of the sprint rather than the end.

Your Role: Ensure developers are writing Unit Tests for their React Native modules.

The Action: In the Daily Stand-up, if a dev says "I finished the code," you ask: "Is it also tested and moved to the 'In Testing' column so the QA team can start?" This prevents a "QA Bottleneck" at the end of the sprint.

B. Dealing with "The Bug Wall" (Days 8–9)
As the Code Freeze approaches, many bugs usually surface at once.

My Role: Triage Facilitator. You lead a quick "Bug Triage" meeting.

The Action: You pull the PO and Lead QA together to look at the bug list. You ask: "Which of these are 'Release Blockers' and which can wait for the next sprint?" You protect the team from fixing minor UI tweaks when they should be fixing critical crashes.

C. Environment & Dependency Management
Testing a mobile app requires a stable backend and identity provider.

Me Role: Blocker Remover.

The Action: If the QA team is blocked because the "Staging Environment" is down, you escalate this to the Scrum of Scrums or the Infrastructure team immediately. QA cannot work without an environment.

D. Definition of Done (DoD) Enforcement
Me Role: The Gatekeeper.

The Action: During the Sprint Review, if a feature is "finished" but wasn't tested on Android physical devices (only on iOS), you declare it "Not Done." You coach the team that in a React Native migration, "Done" means verified on both platforms.

3. Special Role: The "Go/No-Go" Decision
On the final day before the Release Management Sync, you host the internal team "Go/No-Go" meeting.

You present the "Quality Dashboard":

How many bugs were found?

How many are still open?

What is the "Test Coverage" for the new React Native code?

My Question to the PO: "Based on this data, are we confident to submit this to the App Store?"

>>> 4. Summary: 
"My role in testing is to ensure Flow and Transparency. I advocate for 'Shift-Left' testing so QA isn't overwhelmed at the end of the sprint. I facilitate Bug Triage to help the PO prioritize fixes before the Code Freeze, and I ensure our Definition of Done is strictly followed so that no un-tested React Native code reaches our users."

\developers  write their own unit tests