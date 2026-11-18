# Documentation rubric

Score the final reader experience in the area touched by the request. Use integer scores from 1
to 10 for each applicable dimension. Apply the page rubric to each changed page and the site
rubric to the assembled changes. Use `N/A` with a reason when a dimension genuinely has no
bearing, such as runnable examples on a prose-only explanation. For a removed page, assess the
replacement route and whether its reader task still has an answer. If triage finds no warrant
for an edit, record the reader impact and supporting evidence.

## On the page

| Dimension | What earns 10 |
| --- | --- |
| Accuracy and evidence | Claims, commands, defaults, limits, and guarantees match the target release or checkout. Scope and exceptions are stated where they matter. Sources support consequential claims and any reported test result identifies what actually ran. |
| Usefulness | A reader in the stated audience can perform the task, make the decision, or look up the contract. The answer appears early and the reader can tell whether it worked. |
| Clarity | Terms, references, actors, and conditions are unambiguous. Names match the product, and readers can tell which option applies and what each step does. |
| Simplicity | The common path avoids avoidable setup, branches, concepts, and choices. Required details appear where readers need them. Optional detail has a clear place to go. |
| Brevity | Each paragraph, example, and callout earns its space. Repeated background and setup are cut or linked. The shortest useful explanation preserves prerequisites, exceptions, and consequences. |
| Readability and scanning | Headings match reader questions, code and expected output are easy to identify, and formatting makes the page easier to scan. |
| Coverage | The page answers the reader questions in its brief, including prerequisites, important limits, and likely errors or recovery where relevant. Named links take readers to the full answers outside its scope. |
| Example fidelity | Examples use the documented interface and version. Readers have the commands, context, placeholders, and clear result needed to reproduce them. Execution or source and fixture checks support what the page promises. |

## Across the site

| Dimension | What earns 10 |
| --- | --- |
| Findability | Starting at the relevant landing page, sidebar group, or adjacent guide, a reader can reach the canonical answer through predictable labels. Direct entry from search gives enough context to orient the reader. |
| Organization and page economy | Pages have distinct jobs. The site uses the fewest pages that keep each job easy to scan and link to. Navigation shows choices readers need at that point. Any split or merge improves an actual reader route. |
| Coverage and handoffs | Each in-scope question has a reachable answer, including version differences, consequential edge cases, and recovery when relevant. Guides, references, and troubleshooting link at the points where readers need more detail. |
| Consistency and continuity | Related pages agree on public names, commands, defaults, and version boundaries. Existing inbound routes and anchors still work or have an explicit replacement. Each shared fact has a canonical location. |

## Calibrate scores and act on them

| Score | Meaning |
| --- | --- |
| 10 | The criterion is met and the evaluator can point to evidence. |
| 8–9 | The reader can complete the task. A specific remaining improvement would save effort or remove ambiguity. |
| 6–7 | A meaningful reader question or step needs correction, more context, or a better route. |
| 3–5 | Readers are likely to guess, take a wrong path, or need another source to finish. |
| 1–2 | The criterion fails for the primary reader task. |

Use `dimension | score | evidence and reader impact | change needed for 10` for each dimension.
Cite the heading, line, reader route, or source assertion. Give actionable edits, including
what to delete, shorten, move, merge, or link when that is the better fix. Mark blocking
findings and state any limits on verification. For site review, walk the affected reader paths
and record the starting point, destination, and where a reader would hesitate or leave.

Block acceptance on incorrect published instructions, unsupported guarantees, broken paths to
required answers, or a missing prerequisite that prevents a supported task. Judge each dimension
on its own. A high score elsewhere cannot clear a blocker. Keep the supported, shorter version
when a proposed addition adds effort without answering a real question. Report any unresolved
findings and score gaps against the final reviewed candidate.
