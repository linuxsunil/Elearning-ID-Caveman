# Authoring and QA

Use this reference for Storyline 360, Rise 360, LMS, SCORM/xAPI, accessibility, or module QA work.

## Storyline production

| Field | Required detail |
|---|---|
| Objects | Exact timeline names |
| Variables | Name, type, default, purpose |
| States | Initial state and allowed transitions |
| Triggers | Event, condition, action, order |
| Layers | Entry/exit behavior and focus |
| Media | Start, pause, replay, captions |
| Completion | Success, failure, retry, resume |
| Accessibility | Focus order, alt text, labels, keyboard path |

Trigger order can change behavior. Never reorder silently.

For JavaScript, preserve code and identifiers exactly. Separate platform triggers from JavaScript behavior. Flag browser permissions, cross-origin restrictions, LMS sandboxing, and unsupported APIs when relevant.

## Rise production

Specify lesson/block sequence, interaction type, media, knowledge checks, continue-button conditions, and accessibility notes. Prefer native blocks when they meet the requirement; use embedded or custom content only when the learning value justifies maintenance and accessibility cost.

## QA passes

1. Functional: buttons, links, layers, states, triggers, variables, media.
2. Navigation: next/back, menu, revisit, resume, branching, locked paths.
3. Assessment: answers, feedback, attempts, randomization, score, pass/fail.
4. Content: accuracy, consistency, spelling, numbers, source alignment.
5. Accessibility: keyboard, focus, labels, alt text, captions, contrast, zoom.
6. Responsive/browser: viewport, supported browsers, touch, orientation.
7. LMS: package launch, completion, score, suspend/resume, reporting.

## Defect format

`ID | Screen | Severity | Steps | Expected | Actual | Evidence | Suggested fix`

- Blocker: prevents launch, completion, or submission.
- High: core path or assessed behavior fails.
- Medium: workaround exists; learning or usability is impaired.
- Low: cosmetic or minor consistency issue.

Record reproducible evidence. Do not mark untested assumptions as defects.

## Lean QA output

Lead with blockers and high-severity findings. Then give totals, affected learning paths, and recommended retest scope. Keep passed checks summarized unless a full test log is requested.
