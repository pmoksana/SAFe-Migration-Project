

As a Scrum Master, you aren't expected to fix the code in the pipeline, but I'm responsible for monitoring # Flow Metrics.
 * ** If the "Lead Time" (the time from code commit to a testable app) increases, my team's agility decreases.

Here is exactly how an SM "checks" the pipeline and handles the "20-minute delay" scenario.

# ## 1. How the SM Monitors the Pipeline
You don't need to be an engineer; you just need access to your team's CI/CD tool >> ( GitHub Actions), GitLab CI, Bitrise, or Jenkins).

The "Dashboard" has a history view showing every "Build" or "Pipeline Run."

The Time Metric: >>  "Duration" column.

Last week: 15 mins.

This week: 35 mins.

The "Stage" Breakdown: Click into a slow build to see which specific step is hanging. In React Native, it’s usually one of these three:

Dependency Install: npm install or yarn install taking forever.

Native Compilation: The "Xcode Build" (iOS) or "Gradle" (Android) step.

Tests: Running the Jest or Detox test suites.

# ## 2. Investigating the "20-Minute Delay" (The Step-by-Step)
When I notice the builds are getting slower, I follow this "detective" process:

Step A: Spot the Trend (The Data)
Before the Daily Stand-up, you check the tool. I see that since Tuesday, every build has jumped from 15 to 35 minutes.

Your thought: "Every developer is losing 20 minutes of productivity 5 times a day. That’s nearly 2 hours per dev!"

Step B: Raise it in the Daily Stand-up
Ask the team:

SM: "I noticed our CI/CD pipeline runs have jumped from 15 to 35 minutes since Tuesday. Does anyone know why? Is it affecting your flow?"

Dev Response: "Yeah, we added a new React Native library for animations, and now the Android build cache keeps clearing itself."

Step C: Quantify and Coordinate (The SoS Move)
In the Scrum of Scrums (SoS), you report this even if it's not a "hard blocker" yet.

SM to DevOps SM: "Our React Native pipeline duration has doubled this week. It’s adding a massive delay to our 'Definition of Done' verification. Can we get a DevOps engineer to look at our caching strategy today?"

# ## 3. Common React Native "Pipeline Killers"

As an SM, you should recognize these common terms so you can discuss them with the Platform/DevOps team:

Cache Invalidation: The pipeline "forgets" previous work and downloads 2GB of node_modules every single time.

SM Action: Ask for "Persistent Caching."

Parallelization: The pipeline runs iOS, then Android, then Web.

* ** SM Action: Ask, "Can we run these stages in parallel (at the same time) to save 15 minutes?"

Flaky Tests: A test fails for no reason, and the dev has to "Re-run" the whole 30-minute pipeline.

* ** SM Action: Facilitate a tech-debt task to fix or remove the "flaky" test.

# ## 4. The "Business Case" for Fixing it

If the DevOps team says, "We are too busy," you use the SAFe "Cost of Delay" argument:

"We have 10 developers. Each dev runs the pipeline 4 times a day. If it takes 20 extra minutes each time, we are losing 13 hours of engineering time every day. Fixing the pipeline for 4 hours today will save us 65 hours this week."

Summary Checklist for the SM:
[ ] Daily: Glance at the CI/CD dashboard. Are the bars Green? How long are they?

[ ] Weekly: Look at the "Mean Time to Recovery" (How long is the build broken?) and "Average Build Duration."

[ ] During Retrospectives: Ask: "Is the tooling helping you or slowing you down?"

In your interview, you can say:

"I monitor our CI/CD pipeline metrics as part of my focus on Team Flow. For example, when I noticed our React Native builds slowed down by 20 minutes, I didn't wait for a dev to complain. I quantified the lost productivity, raised it in the Scrum of Scrums, and worked with the DevOps team to optimize our build caching, effectively giving the team back hours of development time per week."