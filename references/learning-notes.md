# Reading Progress Guide

Read when showing a visual reading map, or when the reader pauses, resumes, or
requests a saved checkpoint. Keep only what is needed to continue coaching.

## Visual Reading Map

Use a short text route or Mermaid diagram showing the paper's main reading units.
Label the map as reading progress, so its arrows are not confused with the paper's
algorithm or task dependencies. Labels follow the teaching language. For example:

```text
[Covered: Problem] -> [Covered: Method] -> [Current: Evidence] -> [Pending: Limits]
```

Use explicit labels rather than color alone. Mark a partly discussed unit as
partial, and preserve important deferred units when the reader takes a detour.
The route is a reading aid, not a required section order or a percentage estimate.
Covered indicates that material has been explained; track observed understanding
separately in the notes. Update the map at major transitions, on resume, or when
requested; omit it for narrow follow-ups unless the location would be unclear.

## Record

- Paper title, source, version, and unavailable material.
- Current section, figure, table, or equation, together with the active question.
- Explicit preferences for language, diagrams, examples, depth, and pace.
- Concept status: introduced, practiced, checked through a specific response, or
  deferred. Include a brief observation rather than an unsupported mastery claim.
- The precise confusion and the explanation or example last used to repair it.
- The running example and its mapping to the paper, so a resumed session keeps
  terminology, variables, and teaching context consistent.
- The next starting point, required prerequisites, and deferrable details.
- Note or diagram locations and sources that require another check.

Checked understanding requires an actual restatement, prediction, or correct
application. Record "I understand" as self-reported understanding. Do not assign
a global ability score or infer lasting mathematical or programming ability from
one mistake.

## Save and Resume

Use the requested location, otherwise `notes/papers/<paper-id>/progress.md` in the
current workspace. Prefer a verified arXiv ID; otherwise create a short,
filename-safe title identifier. Never use an untreated paper title as a path.

Update only this paper's record. Retain important misconceptions and corrections;
compress long history to the facts needed for resuming. For a conversational
pause without a save request, a copyable checkpoint is enough.

On resume, confirm the paper and record, then explain the previous location and
new starting point briefly. Avoid restarting the whole paper. New questions take
priority; the saved plan supplies context rather than enforcing an old sequence.

## Coaching Feedback

When requested, keep feedback beside the paper's progress record, with the
reader's concrete observation and its effect on the lesson. Distinguish missing
skill guidance, failure to follow existing guidance, and an unresolved issue.
Record useful counterexamples without labeling them automatically as mistakes.
Preserve a requested delay until the reading is finished, unless the reader
explicitly authorizes a particular change sooner. At review, merge related issues
into a few reusable changes and state what was changed and actually verified.
