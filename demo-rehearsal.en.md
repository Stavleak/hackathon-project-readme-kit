# Rehearse a hackathon demo without the author at the keyboard

Stavleak

If a teammate can present the slides but cannot run the submitted version, the demo depends on its author being available. Use this rehearsal before the deadline to find the missing instruction, permission or sample input while there is still time to fix it.

## Choose one route and one result

Write one sentence: “Starting with [sample input], a reviewer follows [steps] and sees [observable result].” A screenshot of the home page is not a result if the project promises to process a request, produce a file or change a record.

Choose the route you actually support: a hosted demo or local execution. If both are available, document each separately. Do not send a reviewer through a local installation guide that ends at an unrelated hosted screen.

- [ ] The submitted commit or version is fixed.
- [ ] The starting input is safe to share and does not contain real participant records.
- [ ] The expected result is specific enough to compare with the observed result.
- [ ] Required accounts and permissions are listed before the first step.
- [ ] Temporary links have an expiry time and an owner who can repair access under the event's rules.

## Hand the instructions to a teammate

The author observes. A teammate starts from the README and uses the environment assigned to the rehearsal. Record every missing step instead of correcting it silently.

For a local route, check the runtime version, working directory, installation command, start command and sample input. List environment variable names and explain where approved test values come from. Keep actual secrets out of the README and terminal recording.

For a hosted route, check the demo link, reviewer permissions, safe test account, starting state and what happens after the main action. A successful browser session belonging to the author does not establish access for a judge.

## Record the first blocked step

Copy this record for one rehearsal. Use a submission reference instead of personal names.

```text
submission_reference:
submitted_version:
route: hosted | local
environment:
sample_input_reference:
steps_followed:
expected_result:
observed_result:
first_blocked_step:
author_assistance_required:
evidence_reference:
next_action:
responsible_role:
rechecked_at:
```

If execution is unconfirmed, write that. A technically valid record can describe an unsuccessful demo. Do not turn “the README was complete” into “the project worked.”

## Repair, then repeat the same scenario

Fix the instruction or access problem in the allowed working version. Repeat the same input and steps so the result can be compared. Retain the first record and note what changed. Follow the event's published deadline and repair procedure when deciding what version may be submitted.

The exercise confirms this scenario in this environment. It does not establish production readiness, every supported input or a competition score. If a recording is the fallback, state what it demonstrates and what still requires a live check.

## Make the final handoff readable

Put the demo route near the top of the README. Keep the fixed version, input, steps, expected result and limitations together. A reviewer should be able to tell what to do next without searching a chat history.

Use the [Stavleak submission acceptance checklist](https://info.stavleak.com/en/guides/hackathon-submission-acceptance-checklist) for the event-side record. The [downloadable acceptance kit](https://github.com/Wezzeso/stavleak-hackathon-acceptance-kit) includes a local structural validator and fictional examples. The check itself remains a human task.
