# The Tensions

These are structural tensions that surface when teams adopt AI agentic coding. They're worth naming because they recur, and because they motivate everything Seam Up proposes.

Not every team will feel all of them equally. Some depend on how your team divides work and how much scope overlap exists between builders. But if you're working with multiple AI-augmented builders on shared projects, most of these will be familiar.

## 1. Parallelism at the wrong layer

Most AI agentic workflows produce a single coherent thread. That thread is powerful _because_ it's coherent. One person holds the full context, and the AI maintains it across the entire arc.

Adding a second engineer to that thread doesn't double throughput. It can fracture coherence.

The old model of "break the project into tasks, distribute tasks" assumed construction was the bottleneck. With AI, _understanding_ and _alignment_ are the bottlenecks. Understanding doesn't parallelize well by splitting a single thread. But it parallelizes very well when you split at the right seam: two builders working on two well-bounded vertical slices, each with their own coherent thread, can move fast without stepping on each other.

The problem isn't multiple builders. It's multiple builders sharing one conceptual thread.

**Symptom:** Adding people to a project can create more coordination overhead than it saves in build time.

## 2. Artifact ownership ambiguity

Engineering artifacts like the spec, design, and task plan tend to cover the whole project scope. But other builders own pieces of that scope. The artifacts either overstep into others' domains (violating their autonomy) or leave gaps (making the artifacts incomplete and potentially missing constraints).

Neither is good. Overstepping breeds friction. Gaps breed surprises.

**Symptom:** Builders aren't sure whether an artifact oversteps into their scope or leaves something out. There's friction at integration that could've been caught earlier.

## 3. Collaboration as interruption

The agentic workflow feels continuous and individual. You're in flow: context is loaded, the AI is tracking your thread, you're moving fast. A collaboration checkpoint, whether it's a sync meeting, a review request, or a "can we align on this?", feels like a context-switch. An interruption to the real work.

But that framing is the problem. Collaboration isn't an interruption; it's an _input_. The issue is that the agentic workflow doesn't have natural places where external input fits in. When collaboration has no home in the flow, it will always feel disruptive.

**Symptom:** Collaboration can feel like an interruption rather than a part of the solution process.

## 4. Expertise leverage vs. execution speed

AI makes solo execution fast. But it doesn't replace the value of diverse perspectives on _what_ to build and _how_ to approach it. There's a real risk of optimizing for speed at the cost of better solutions. If everyone is heads-down doing deep solo work with AI, when do you actually leverage each other's expertise?

This tension predates AI. Shape Up already leans toward small teams with high autonomy. AI accelerates the trend but doesn't cause it. The real question is: where does collaboration actually improve outcomes vs. where is it a coordination tax?

**Symptom:** Everyone's moving fast individually, but the outcomes aren't better than when you collaborated more.

## 5. Speed amplifies wrong paths

AI doesn't just make you faster on the right path. It makes you faster on the wrong path too.

Without upfront alignment on approach and boundaries, a builder can generate a significant amount of structurally wrong code before anyone notices. The code works. The tests pass. But the approach doesn't fit. It conflicts with another builder's scope, makes assumptions about an agreement that hasn't been made, or solves the problem in a way the team wouldn't have chosen with more context.

Code review becomes the moment of reckoning. Instead of catching style nits and edge cases, reviewers find structural misalignment. That's an expensive place to discover disagreement. The code might need to be reworked or thrown away, and the speed that generated it just made the waste larger.

**Symptom:** PR reviews regularly surface structural surprises. Style notes and polish are expected in review. Structural direction should not be.

---

These tensions aren't catastrophic on their own. Teams work through them every day, often without naming them. But they compound. And they all point in the same direction: the seams between builders' work are where things go wrong when AI accelerates individual execution. Next we'll lay out the principles for getting the seams right.

---

Prev: [Background](02-background.md) | Next: [Guiding Principles](04-principles.md)
