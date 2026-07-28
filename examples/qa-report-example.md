# QA report example

## Summary

- Blockers: 0
- High: 2
- Medium: 1
- Low: 1
- Retest: quiz submission, revisit navigation and LMS resume

## Defects

| ID | Screen | Severity | Steps | Expected | Actual | Suggested fix |
|---|---|---|---|---|---|---|
| QA-01 | Quiz 3 | High | Select B → Submit | Incorrect feedback appears; attempt decreases | Correct layer appears; score increases | Correct answer mapping and retest scoring |
| QA-02 | 2.4 | High | Complete slide → Back → Next | Return to 2.5 | Next remains disabled | Re-evaluate disabled state on revisit |
| QA-03 | 1.2 | Medium | Tab through interaction | Focus follows visual order | Focus jumps from button 1 to button 4 | Correct focus order |
| QA-04 | Menu | Low | Open menu at 200% zoom | All labels remain visible | Final label clips | Increase responsive text area |

## Passed checks

Audio controls, captions, first-attempt navigation and course completion passed.

## Retest scope

Retest affected slides, quiz score, pass/fail status, suspend/resume and completion reporting in the LMS.
