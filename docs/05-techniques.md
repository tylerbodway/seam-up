# Techniques

With the guiding principles in mind, these techniques describe how to put those values into practice within AI-augmented workflows.

Some are team activities, some are personal workflow choices. Each technique notes which it is.

## 1. Layered artifact production

**Personal workflow.** Structure your AI planning workflow to produce artifacts at two explicit layers:

**Shared layer** (goes through team collaboration):

- Engineering spec distilled from the product spec
- Scope agreements at each seam (interfaces, data shapes, integration points)
- Scope map (who owns what, with explicit boundaries)

**Personal layer** (internal to you):

- Design decisions within your scope
- Task plan and implementation steps
- AI context documents (system prompts, codebase notes, working memory)

AI workflows generate artifacts constantly. Without a clear layer separation, everything feels like it needs review, or nothing does. Be explicit: shared-layer artifacts are what you bring to the team, personal-layer artifacts are yours to iterate on freely.

## 2. Shaping with pre-work

**Team activity, with individual preparation.** This is the highest-leverage technique in practice. It changes what a shaping session is for: instead of generating ideas from scratch as a group, you refine and challenge a concrete starting point.

Before the collaborative shaping session:

1. Use your AI workflow to distill the product spec into a draft engineering spec.
2. Identify the obvious scope boundaries and draft initial seam definitions.
3. List open questions and decisions that need other perspectives.

Share this as pre-read. The shaping session then focuses on refining the seams, challenging assumptions, and incorporating other builders' constraints, rather than starting from a blank page.

Two things to get right:

**Keep the draft rough.** The pre-work should be a starting point, not a finished plan. If it's too polished, you miss out on the expertise and perspective your teammates would have contributed to the initial thinking. General ideas and open questions are better than detailed proposals.

**Frame it as a draft.** Make it clear that the pre-work is input to the shaping session, not output from it. The session's job is to reshape, challenge, and improve the draft, including throwing parts of it away.

## 3. Scope splitting at the seams

**Team activity.** Before anyone starts building, run a focused session to define scope agreements at each seam:

1. Take the engineering spec.
2. Identify the natural vertical slices (Shape Up's scopes).
3. For each pair of adjacent scopes, define the seam: what data crosses it, what APIs exist, what events are emitted, what assumptions each side can make.
4. Each builder takes their scope(s) and runs their own workflow independently.

This is where Shape Up's vertical slicing directly applies. The AI workflow enhancement is that you can use AI to rapidly prototype the scope agreements and validate them before anyone builds. Draft the interfaces, mock the data shapes, even generate stub implementations to test that the seams hold, all before committing to real code.

The goal isn't exhaustive specifications. It's making the seams explicit enough that two builders can work independently without stepping on each other.

## 4. Seam-change proposals

**Team activity.** When your AI workflow surfaces a seam change mid-implementation (an API shape needs to shift, a data model doesn't work as expected, a new constraint affects another builder's scope), formalize it:

1. Draft a short change proposal: what changed, why, and the impact on other scopes. AI can help you write this quickly.
2. Discuss it personally or post it to whatever channel your team uses.
3. The affected builder reviews and can either acceps, negotiate, or push back on the change.
4. Update the scope agreement.

This keeps the agentic flow mostly uninterrupted. Draft the proposal quickly, post it, and continue working on non-blocked parts of your scope. The key is that seam changes don't sit in someone's head. They surface promptly because the cost of delay compounds.

---

Prev: [Guiding Principles](04-principles.md) | Next: [Getting Started](06-getting-started.md)
