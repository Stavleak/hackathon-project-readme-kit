# [Project name]

A Stavleak template for a hackathon project's README.

Replace the bracketed fields with the results of your own check. Remove settings that do not apply and the sample scenario if it does not match your project. The `text` blocks below contain fields to complete, not ready-to-run installation commands. Do not add passwords, tokens or personal data.

[Русский](README.ru.md) · [Қазақша](README.kk.md)

## Task and current state

- User: [role without personal data].
- One task: [specific action].
- Result: [what the person sees or receives].
- State: [working prototype; unfinished parts].
- Implemented: [features you checked].
- Stubs: [what is shown for demonstration].
- Not implemented: [what is missing].
- Repository: [approved link].
- Demo: [accessible address and corresponding version; or local route].
- Help: [approved event channel or team role].

## Versions and primary setup route

```text
route: [local | hosted | hardware]
runtime_versions: [checked runtime versions]
dependency_manager: [name and checked version]
external_dependencies: [required services or none]
working_directory: [directory for commands]
install: [installation command using the saved lockfile]
configure: [configuration setup without exposing secrets]
load_demo_data: [tested command or manual step]
start: [tested command or steps to open the demo]
ready_when: [observable sign of readiness]
```

Add an expected sign of success for each step and a known error if you encountered one during testing. Follow the sequence in a clean environment. Check someone else's code in a disposable isolated environment without work secrets or host-folder mounts.

## Settings without secret values

Keep only names your application actually uses. For each one, give its purpose, whether it is required and the agreed way to obtain the value.

- `APP_MODE`: [application mode; whether needed for the demo].
- `DEMO_DATA_PATH`: [path to safe sample data].
- `SERVICE_API_KEY`: [only if needed; how to get restricted test access, without the key value].

The example configuration file should contain safe public settings and placeholders. Share real secrets separately through an approved channel.

## Input and expected result

```text
input_reference: [file or exact request body]
action: [screen and control, or API method and route]
expected: [specific response or observable result]
comparison: [comparison rules, order and accepted fields]
no_match_or_invalid_input: [input and expected behavior]
```

Illustrative example for a room filter. The data is fictional and describes no real rooms or bookings. Replace it with your scenario.

Starting data:

```json
{"rooms":[{"id":"demo-room-a","equipment":["projector","whiteboard"]},{"id":"demo-room-b","equipment":["projector"]}]}
```

Input:

```json
{"required":["projector","whiteboard"]}
```

Expected response:

```json
{"rooms":["demo-room-a"]}
```

The input `{"required":["microphone"]}` expects `{"rooms":[]}`.

## Reset and repeat

- Reset: [command or steps restricted to test data].
- Starting state: [what is restored].
- Reset confirmation: [what to check].
- Repeat run: [same input and observed result].
- If the result changes: [conditions, available versions and saved responses].

## Access and limitations

- Code, data and recording open with judge permissions: [check result].
- Invitation and access expiry: [conditions or not_required].
- Test login: [how to obtain it through an approved channel, without a password].
- External service unavailable: [observed behavior].
- Backup recording: [approved link; what it shows and what it does not confirm].
- Limitations: [untested formats, data, devices and scenarios].
- For AI: [available model versions, prompt, settings and references to safe raw responses; or not_applicable].

## Criteria and contribution

- Event criterion: [exact name].
- Verifiable evidence: [file, scenario or result].
- Team work: [what was implemented during the event].
- Starting components: [existing code, libraries and source].
- Assistance and AI use: [disclosure under the published rules].

## Check record outside the final commit

Update the README, create the final commit, then record its full identifier in the submission form. Save the README permalink after creating the commit as well. Do not add the identifier of the commit containing the README to that same file: saving the change would require another commit.

Complete the following block separately in the event's approved working space after the check:

```text
submission_commit: [full identifier]
readme_permalink: [README in the specified commit]
checked_environment: [runtime and versions]
input: [safe input]
steps: [sequence performed]
expected: [expected result]
observed: [actual result]
blocked_at: [specific step or none]
author_assistance: [help needed or none]
limitations: [what is unconfirmed]
```

A technical check does not determine a competition score or confirm production readiness.

## Stavleak materials

[Rules](https://info.stavleak.com/en/guides/pravila-hakatona) · [Criteria](https://info.stavleak.com/en/guides/kriterii-ocenki-hakatona) · [Submission acceptance](https://info.stavleak.com/en/guides/hackathon-submission-acceptance-checklist) · [AI demo evaluation](https://info.stavleak.com/en/guides/proverka-ai-prototipa-do-pitcha)
