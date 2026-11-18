# Subagents-driven documentation

The lead owns scope, page boundaries, navigation, and acceptance. Use the database repo's
approach of exclusive ownership, parallel work, independent review, and final integration.
Follow the current harness's delegation and concurrency rules.

## Prepare and dispatch

1. Keep a temporary Markdown ledger outside the tracked docs tree. Record the source base and
   target, docs starting state, and a table with page or route, reader question, owned file,
   dependencies, acceptance checks, agent, status, and reviewed snapshot. Reconcile it with Git
   and the harness if work resumes after an interruption.
2. Agree on page titles and routes, where each answer lives, terms and version boundaries, and
   what adjacent pages may link to. Assign each changed or new page to its own writer, including
   small changes when they are in scope. Treat a removed page as its own assignment and include
   its replacement route or the reason the reader task is obsolete. The lead owns `docs.json`,
   redirects, and other shared files. If a shared content file is also a changed published page,
   give it a designated writer and coordinate any further edit with that writer.
3. Dispatch all independent writers in parallel up to the available slots. Queue one assignment
   per remaining page and start it as a slot frees. Give each writer exclusive ownership of one
   path in a shared checkout. Keep shared-checkout edits unstaged and integrate isolated outputs
   according to the harness rules. Narrow or sequence assignments that still depend on an
   unresolved decision while the others proceed.

For each writer, give the user request, one owned page, the reader and their task, required and
out-of-scope questions, agreed routes and terminology, the source range and relevant evidence,
and page-specific acceptance checks from the [rubric](rubric.md). Point to the existing page and
only the neighbors the writer needs. Ask for the edit, the claims and evidence checked, any
examples run, and unresolved questions. Tell writers to leave shared files to the lead and
handle only their assigned page.

## Review the assembled draft

1. After the writers finish, integrate the drafts and update shared site files as needed. If
   integration reveals another page that needs a link or revision note, add it to the page plan
   and assign its writer. Capture the exact docs snapshot or diffs, including new files. Use
   that candidate for the entire review round.
2. Dispatch a fresh, read-only evaluator per changed or removed page. Use isolated conversation
   context, including when the evaluator reads the shared checkout. Give each evaluator the user
   request, the page brief, rubric, current page and page diff, relevant source evidence, and
   the surrounding routes or snippets needed to assess placement. Exclude writer commentary,
   prior scores, and other evaluator feedback. Ask for an independent score and concrete changes
   needed for 10 on every applicable dimension.
3. Dispatch a separate fresh, read-only evaluator for the integrated site. Supply the affected
   reader questions, revised page set, navigation and redirect diffs, adjacent unchanged entry
   points, and any applicable release constraints. Ask them to follow the routes from a reader's
   starting point and score the site dimensions. Individual page reviewers can flag placement or
   overlap. The site evaluator checks those issues across the assembled changes.

## Revise and accept

- Record scores and findings against the exact reviewed files. Resolve factual, task-blocking,
  and navigation defects first. Assign substantive page revisions back to their writer or a
  fresh writer if needed. The lead can apply small, agreed fixes after writing settles. Resolve
  competing feedback against the source and an explicit reader task. Tie each revision to a
  concrete improvement.
- After revisions, dispatch a fresh evaluator for every page whose content or review context
  changed and rerun the site review when reader routes, coverage, or shared contracts changed.
  Reuse scores for pages whose reviewed snapshot and relevant context still match. Recheck the
  integrated result with the site's validation commands.
- Aim for 10 on every applicable dimension. Continue while a concrete, worthwhile in-scope
  improvement remains. If a score stalls, identify the missing evidence or try a specific
  alternative grounded in the reader task. When further gains depend on missing evidence, extra
  scope, or a tradeoff that would worsen the docs, record the lower score, what would earn 10,
  and what prevented it. Acceptance requires the rubric's correctness and usability checks.
- Queue work when slots are temporarily full. If the harness cannot supply a delegate for a
  role, complete that work in the lead context and report which pages or site checks lack
  independent review. Keep the ledger, briefs, and scores out of published pages.
