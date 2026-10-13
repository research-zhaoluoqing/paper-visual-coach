# Visual Explanation Guide

Read when creating an HTML notebook, an interactive explanation, or choosing a
visual representation. Use a static diagram when interaction adds no insight.

## Choose a View from the Question

| Reader's question | Useful view | Required content |
|---|---|---|
| How does an input become an output? | Flowchart | Inputs, operations, outputs, conditions, feedback direction |
| Why does execution take this branch? | Task or search tree | Current node, candidates, selection rule, termination state |
| What changes in this step? | Before/after view or state table | Previous state, operation, next state, fixed conditions |
| How do two methods differ? | Side-by-side views of the same example | Shared input and evaluation conditions; no invented differences |
| What does each equation term do? | Equation annotations and a numerical table | Original formula, symbols, units, a valid calculation |
| Which conclusion does an experiment support? | Question/setup/result/conclusion view | Dataset, metric, baseline, values, limitations |

Choose the representation from the current example before choosing tools. Label
spacing or area as schematic when it does not represent measured quantities.

## One Visual Reading Unit

State the diagram's question before showing it, then explain the important arrows
through the same example. A common arrangement is a plain-language statement,
concrete instance, main view, necessary detail, source location, and one
understanding question. Use this as guidance, not a mandatory layout.

For "switch routes after failure," a teaching task could be finding a specified file:

```text
Find the file
 |-- Current directory: absent -> this branch fails
 `-- Another directory: found -> stop searching
```

Clarify whether nodes are tasks or actions in the actual algorithm. This example
only illustrates branch switching; it does not establish any paper's method,
performance, or search policy. Map it back to the actual algorithm, including
whether the algorithm attempts the whole task before generating branches.

## Add Interaction Only for a Learning Question

First name the reader's action and expected insight: for example, "click Next to
observe how failure changes the current node." Useful interactions include
stepping through a trajectory, comparing methods, exploring a branch, and changing
parameters that may legitimately vary in a formula.

Do not invent experimental values when sliders move. Simulate rules stated in the
paper or clearly labeled teaching simplifications. Provide an initial state,
reset, current state, and important variables. Check a normal path, a failure
path, and a termination condition. Do not autoplay an endless animation.

Understanding checks default to open questions. Hide answers or reveal them after
the reader responds; do not automatically show them beside the question.

## HTML Delivery

- Use one self-contained HTML file with inline styles, teaching SVGs, and small
  scripts. Handle other media according to the environment's access rules.
- Keep core explanations and static states readable without scripts and offline.
  Do not require either inspiration repository's renderer.
- Use readable text in the selected teaching language and scalable diagrams.
  Check narrow screens for overflowing cards, equations, or arrows; split dense
  diagrams into connected views.
- Communicate state through text and shapes as well as color. Label controls and
  support keyboard interaction.
- Typeset mathematics correctly using available rendering tools or suitable local
  dependencies. Without a math renderer, use HTML/SVG for simple expressions;
  for complex ones, use a verified image of the original equation with symbol
  explanations. Unrendered formula source is not a finished explanation.
- Put source evidence in an expandable area with version, section, figure, table,
  and equation locations. Label original figures, redraws, and teaching examples.
- Preview the first screen, a dense diagram or equation, and the ending. Actually
  exercise interactions and check their state transitions.
- When preview tools are unavailable, perform the structural checks you can and
  disclose missing visual or interaction validation. Do not claim all checks passed.

Save to the reader's chosen directory. Otherwise, when saving is requested, use
`notes/papers/<paper-id>/` within the current workspace for `reading.html` and
Markdown source notes on the same topic. Confirm the directory stays within the
workspace and preserve other materials. A single concept question can be answered
with a diagram in the conversation without creating HTML.
