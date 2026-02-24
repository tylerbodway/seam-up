# Guiding Principles

Where the tensions describe where it goes wrong, these principles describe how to get it right. They're guidelines, not rules. Adapt them to your team's context.

## 1. Collaborate on seams, not internals

The highest-value collaboration is at the seams between builders' work, not inside it. Agree on things like:

- Quality criteria and acceptance conditions
- Scope boundaries (who owns what)
- Domain modeling, data, and APIs
- Component interfaces and state ownership

Everything inside a scope is owned by whoever holds that scope. Their workflow, their approach, their problem-solving. This respects autonomy while ensuring coherence across the project.

Spend collaborative energy on defining the spaces _between_ scopes, not on co-constructing within them. When the seams are well-defined, builders can move fast and independently. When they're not, speed creates divergence.

## 2. Separate shared and personal artifacts

AI workflows generate a lot of artifacts. Not all of them are for the team. Be explicit about which are shared (for the team) and which are personal (for you):

**Shared artifacts** go through team collaboration and need alignment:

- Engineering spec (all builders)
- Scope agreements at each seam (builders whose scopes touch)

**Personal artifacts** are yours to iterate on freely:

- Scope plan and design decisions
- Task plan and implementation steps
- AI context documents

That said, the line isn't rigid. Design decisions from your personal layer can and should be raised to the team when it would be helpful, whether you want feedback on an approach or want to make sure your direction aligns with someone else's scope. The layers just make it clear which artifacts _require_ coordination and which don't.

This also extends to how teams agree on how to work together. Beyond the scope agreements themselves, it helps to have a lightweight meta-agreement:

- **What** shared artifacts does this project produce? At minimum, an engineering spec and scope agreements at each seam.
- **When** do collaboration checkpoints happen? After shaping, at seam changes, at integration.
- **How** are seam changes communicated? Async proposal, review, accept or renegotiate.
- **Not prescribed**: how individuals produce their internal artifacts, what tools they use, or what their personal workflow looks like.

This gives the team a common protocol without prescribing individual workflows.

## 3. Draft, shape, build, review

Four phases, each with a different collaboration mode:

- **Draft** (individual): Use your AI workflow to prepare a rough starting point before shaping. Distill the product spec, identify obvious scope boundaries, and list open questions. Share this as pre-read so the shaping session has something concrete to react to. Keep it rough. If it's too polished, you miss out on the expertise your teammates would have brought to the initial thinking.
- **Shape** (collaborative): Refine the draft together. All builders contribute domain expertise. Challenge assumptions, incorporate constraints, and agree on scope boundaries and seam agreements. This is where diverse perspectives are most valuable, before committing to decisions that constrain everyone's work. This can happen synchronously or asynchronously, whatever fits your team.
- **Build** (individual): Each builder works their scope with their own workflow. Communicate through the agreed scope agreements. Surface blockers or seam changes async.
- **Review** (collaborative): Code review, integration, scope check-ins. If shaping was done well, review should surface polish, not structural surprises.

Collaboration bookends the building phase rather than running through it. Shape well enough that building can happen independently. Review to confirm the seams held.

## 4. Artifact update cadences

Not all artifacts update at the same speed, and that's a feature, not a problem. From the broadest team artifacts down to the most personal:

- **Engineering spec**: Updates at major checkpoints. This reflects the team's current shared understanding of the project. Changes here are significant.
- **Scope agreements**: Update only through a proposal process. These are shared artifacts at the seams. Changing them unilaterally defeats the purpose.
- **Design decisions**: Update as you learn. Raise relevant ones to the team at review checkpoints or when they touch a seam, but don't wait for approval to explore.
- **Task plan**: Updates constantly. This is your personal workflow. Iterate freely, reorganize, reprioritize. No one needs to review your task plan.

The encouragement here is to move fast on your personal layer. The AI workflow lets you rapidly iterate on your task plan, explore design options, and restructure your approach without coordination overhead. That speed is the whole point of individual autonomy within well-defined scopes. The only artifacts that need coordination are the ones at the seams.

## 5. Seam changes are the highest-priority communication

When a builder discovers something that changes a seam, whether it's an API shape that needs to shift, scope that needs to move between builders, a technical constraint that affects someone else's work, or a new solution approach that changes the agreed design, that's the one thing that should surface quickly.

Not because process demands it, but because it's practical. A seam change can block another builder's flow. It can mean scope needs to be re-shaped. It might mean going back a step to collaborative design when a new constraint or idea emerges. The longer a seam change goes uncommunicated, the more work builds on an outdated agreement.

Everything else (status updates, internal design decisions, task progress) flows through normal async channels. Seam changes get elevated because the cost of delay is highest there.

---

These principles point toward a way of working, but they don't prescribe the mechanics. Next we'll cover practical techniques for putting them into practice.

---

Prev: [The Tensions](03-tensions.md) | Next: [Techniques](05-techniques.md)
