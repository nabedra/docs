---
name: nabedra-documentation
description: Write, revise, and review the Nabedra Mintlify docs. Use when a change in nabedra-database may need a docs update, or when asked to improve a Nabedra page, example, or navigation path. Checks reader impact, assigns one writer and one independent evaluator per changed page, and scores the integrated docs against a rubric.
---

# Nabedra documentation

Lead each run. Find the smallest set of edits that lets readers complete the tasks and make the
decisions affected by the request. If the user asks whether a database change needs better docs,
make the warranted updates. For an explicit audit-only request, report findings and proposed
edits.

## Decide what readers need

1. Read `docs.json`, the source revision in `index.mdx` and `README.md`, and the affected pages.
   Use the requested PR, commit range, branch, or checkout when given. Otherwise inspect the
   sibling `../nabedra-database` checkout and compare the documented revision with its current
   state. Inspect `git status --short` so relevant staged, unstaged, and new files enter the
   comparison. In another workspace, use the available checkout or the `zPy52/nabedra-database`
   remote. Record the base, target, and any uncommitted scope. Leave the source checkout as you
   found it. If evidence is missing, carry on with claims you can verify and report the gap.
2. Inspect the diff and trace affected behavior to implementation, public types, CLI help,
   tests, and release evidence as appropriate. Treat plans and acceptance contracts as
   statements of intent. Distinguish published releases, checkout-only behavior, and proposals.
   Read the upstream `AGENTS.md` and linked evidence when a change touches worker execution,
   recovery, or other covered areas.
3. For each change, name what a reader now needs to do, decide, expect, or look up. API and CLI
   changes, setup and defaults, limits, compatibility, migration, and operational behavior can
   warrant edits. For an internal refactor or a routine fix that restores documented behavior,
   skip the guides. Use an existing changelog only for fixes readers need to know about. If a
   fix changes an instruction, invalidates a workaround, or changes an operational decision,
   update the affected page. When no reader-facing change warrants an edit, report the range
   checked and why the docs still hold.
4. Map each changed reader question to one canonical answer. Update an existing section first.
   Create a page only when it answers a distinct task or lookup and would make the current page
   harder to use if kept there. Plan the reader's route to the answer, any links or redirects,
   and how the old page fits. Read the [rubric](references/rubric.md) before dispatch so the
   briefs include the right checks.

## Put the common path first

- Aim for the 20% of details that deliver 95% of the value on the first read. Give the answer,
  recommendation, or first action early. Keep prerequisites, conditions, and costly failure
  modes next to the action they affect. Put optional branches, exhaustive parameters, and rare
  recovery paths within reach in a named section or linked reference.
- Give each page a dominant job. A quickstart gets to a confirmed result. A how-to solves a
  task. A reference lets readers look up exact behavior. An explanation supports a decision or
  mental model. Link between these jobs at the point the reader needs to switch.
- Use task and lookup words in titles, headings, and links. Write in plain, direct sentences and
  use the public names readers will see in code, output, or configuration. Cut repeated setup,
  filler, and unnecessary callouts or navigation choices. Use tabs only for equivalent paths,
  such as different supported environments for the same step.
- Show the smallest example that proves the point. State where to run it, versions or setup that
  matter, what to substitute, and what success looks like. Check commands and code against the
  intended release or revision. Keep exact defaults, units, limits, and errors where readers can
  find them.
- For specific models of onboarding, examples, navigation, and reference pages, consult
  [documentation examples](references/documentation-examples.md) when shaping a new page or
  resolving a design tradeoff.

## Write, review, and verify

Follow [subagents-driven documentation](references/subagents-driven-documentation.md) when
pages need writing. The lead assigns one writer per page and then assigns a fresh, read-only
evaluator to each changed page. Evaluate the assembled site changes too. Revise the drafts and
repeat the relevant reviews until the rubric passes or remaining improvements depend on a
specific blocker or tradeoff.

Use frontmatter and components consistent with nearby MDX and root-relative links such as
`/python/connect`. Register new public routes in `docs.json` and preserve existing URLs and
anchors where possible. Update the pinned revision in `index.mdx` and `README.md` together only
if the resulting site can support that updated claim. Qualify narrower or unreleased changes on
the affected pages and keep historical evidence pinned to the revision that produced it. When
behavior exists only in local changes, record that scope in the handoff and keep release claims
tied to versions readers can identify.

Verify the final diff with `git diff --check`, `mint validate`, and `mint broken-links`. Check
affected anchors and redirects when routes or headings change. Run changed examples against the
intended version when practical. Record exactly what ran and what remains unverified. Report
what changed or why no edit was warranted, the source scope, the final page and site scores for
edits, and any remaining issue with the change that would address it.
