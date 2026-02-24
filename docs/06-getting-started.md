# Getting Started

Seam Up doesn't need to be adopted all at once. Start where you are, try one thing, and see if it helps.

## Phase 1: Separate your layers

Start now, no process change required. When you produce artifacts in your AI workflow, be explicit about which are shared (for the team) and which are personal (for you).

This might start as something you do individually as you're gauging team interest. You don't need buy-in to start separating your own artifacts into shared and personal layers. Communicate the idea in whatever way works best for your team context. Elevating it to a team standard may take time, and that's fine.

You'll know this is working when the question "does this artifact need review?" stops coming up. The layer makes it obvious.

## Phase 2: Split scope at the seams

Try this on your next project. Before anyone starts building, run one shaping session to define scopes and the agreements at each seam. Use AI-generated pre-work to give the session a concrete starting point, but keep it rough. The session's job is to refine, not to rubber-stamp.

After shaping, each builder takes their scope and works independently. Communicate through the agreed seam definitions.

You'll know this is working when builders can make progress on their scopes without waiting on each other, and integration points connect without surprise rework.

## Phase 3: Formalize across the board

Over time, formalize the patterns that work. This is about establishing consistency so new projects follow a familiar flow:

- Standard artifact locations and formats
- Clear review processes for shared artifacts
- Defined proposals when seam changes happen mid-build
- Consistent shaping sessions with pre-work before each project

The goal is that the team's collaboration patterns become reliable and repeatable, not that they become bureaucratic. Keep it lightweight.

You'll know this is working when starting a new project doesn't require reinventing how the team collaborates. The patterns are just how you work.

### Real-world tooling

The specifics depend on your team, but here are examples of how teams could put this into practice:

- **Document databases** (e.g. Notion) for engineering specs, scope agreements, and project documentation
- **Discussion and announcement posts** (e.g. GitHub Discussions, Asana) for async seam-change proposals and shaping pre-reads
- **Committed project files** (e.g., `docs/projects/:slug/`) for version-controlled specs and scope agreements, reviewed through PRs
- **Task management** (e.g. Asana) for status updates and tracking within individual scopes
- **Chat channels** (e.g. Slack) for quick async coordination and surfacing seam changes that need attention
- **Code review** (e.g. GitHub PRs) for the review phase, where structural alignment is confirmed

## Summary

Seam Up preserves Shape Up's strengths (shaping, appetite, vertical slicing, scope hammering) and evolves the building phase for AI-augmented builders who can each hold larger individual scopes.

The core moves:

1. **Shape the seams.** Collaborative energy goes to defining the agreements between scopes, not co-constructing within them.
2. **Build within scopes.** Each builder has full autonomy and accountability within their scope, using whatever workflow works for them.
3. **Communicate at the seams.** Seam changes are the highest-priority, most-structured communication. Everything else flows through normal async channels.

## AI skills

This repo includes installable AI skills as a starting point to operationalize the techniques from this book. See the [skills directory](../skills/README.md) for what's available and how to install them. You'll likely want to tweak them to suit your tooling/workflows better.

---

Prev: [Techniques](05-techniques.md)
