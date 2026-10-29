# Source-backed evidence retention verification

## Status

Implementation and all 15 Change tasks are complete. Local verification and the Windows/Linux CI suites passed. CI is not fully green: two macOS jobs were cancelled before acquiring a hosted runner; those remote checks remain unverified.

## Delivered surface

`src/core/templates/evidence-retention.ts` supplies one shared instruction block. The explicit consumer list is in design Decision 1. A normal built-CLI `init --tools omp --profile full` into an isolated project with spaces in its absolute path installed all 23 affected consumers with exactly one block each. `update` reported those installations up to date. Inspection of the installed planning, benchmark, verification, archive, and review-cycle skills confirmed Store selectors, report-only dispatch, standalone destinations, and existing verdict/test-evidence boundaries remain present.

This changes generated agent guidance, not enforcement: there is no recipe executor, validator, data migration, or new archive gate. No claim is made that every model will follow the instructions.

## Executed checks

Environment: macOS arm64; Node `v24.18.0`.

- `pnpm run build` — passed.
- `pnpm exec tsc --noEmit && pnpm lint` — passed.
- `env -u ZSH pnpm exec vitest run test/core/templates test/core/shared/skill-generation.test.ts test/core/shared/skill-sidecar-install.test.ts test/core/workflow-generation-integration.test.ts test/core/file-placement.test.ts test/core/workflow-chain.test.ts test/core/archive-consumer-integration.test.ts` — 16 files, 135 tests passed. Includes real init/update installation and generated archive argv executed through Commander.
- `env -u ZSH pnpm exec vitest run test/source-byte-hygiene.test.ts` — 5 tests passed; the removed template file has no remaining byte-hygiene exception.
- `RASEN_LANG=en node bin/rasen.js validate source-backed-reproducible-evidence-retention --strict` — valid.
- Actual CLI init/update and recipe commands used an isolated HOME/XDG scope and an explicit temporary repository base containing spaces. No host install was refreshed.
- Frozen template hashes and wording/copy assertions were removed from `skill-templates-parity.test.ts`, not re-pinned. No new permanent prompt-string tests were added.

## CI result

[CI run 40917684178](https://github.com/pashifika/rasen/actions/runs/40917684178) tested commit `dcaca6f88842e690e0a1c58df339ef2e6f916807`.

| Surface | Result |
| --- | --- |
| Windows PowerShell tests, shards 1/3, 2/3, 3/3 | Passed, including the focused Windows path checks in shard 1 |
| Windows file-placement recovery and layout migration | Passed |
| Linux full suites, Node 20.19.0 and Node 24 | Passed |
| Linux file-placement recovery and layout migration | Passed |
| macOS layout migration | Passed |
| macOS full suite and file-placement recovery | Cancelled before execution: hosted runner unavailable |
| Lint/type check, UI package build/tests, Nix validation | Passed |

GitHub's cancellation annotation was `The job was not acquired by Runner of type hosted even after multiple attempts`, with macOS arm64 capacity warnings. The run conclusion is `failure`; aggregate gates were skipped. Local macOS checks are reported separately and are not substitutes for the cancelled remote jobs.

## Scenario evidence

| Scenarios | Delivered guidance / exercised check |
| --- | --- |
| Deterministic fixture; explicit claim and stopping scope | Shared claim-first/mode clauses. A disposable committed generator ran twice with seed `evidence-v1`; both outputs had SHA-256 `132b22bbad2d1bbb1c2c30bd9dd42eaa172f0219d4d29e6df0fe56dc65bce3bc`. A different seed changed the output. |
| Historical reanalysis; aggregates, failures and incomplete attempts | Four synthetic observations were retained once: three numeric observations and one timeout. Two analyses returned `observed=3`, `failed=2`, `mean=15`, `max=20`, `verdict=fail`. The 70-byte summary contained no observation array; input bytes stayed unchanged. These are fixture values, not product performance measurements. |
| Distribution evidence | Guidance explicitly retains samples and exclusion meanings; aggregates are not substitutes for required samples. No percentile benchmark was claimed or run. |
| Separate analysis/measured identities; dirty source | Recipe guidance and the documentation template name both identities. A local source deviation left the fixture HEAD unchanged; its diff digest was `74803784907ceb78a9745fd59a8f908e0492c5dc3d6a9afef53c394d81a01288`. A commit alone therefore did not identify the executed source. |
| Changed, missing and private inputs | Changing the observation input changed its digest and mean to 45. An unavailable input produced `ENOENT`. An inspection-only private-reference example explicitly reported unavailable receiver access and unverified reproduction; no real private payload was used. |
| Variable metadata; new timing observations | Two fresh 10,000-hash timing runs produced distinct run IDs and elapsed values (10.072416 ms and 10.388917 ms). Only `stable.iterations=10000` was compared as stable; neither run replaced the historical fixture input. This illustrates mode separation, not a performance claim. |
| Recorded commands are data | Read an untrusted recipe containing a harmless file-creation canary command without executing it; the canary remained absent. This is a manual read-only inspection smoke, not a sandbox or automatic-execution guarantee. |
| Path bases and platform meaning | Actual generation and recipe execution succeeded from an explicit macOS repository path containing spaces. Documentation uses argument-vector boundaries, not an assumed POSIX shell. Windows generation/installation, path, and placement coverage ran in the successful CI shards; the disposable recipe itself ran only on macOS. |
| Dispatched/standalone reports; legacy reports and immutable archives | Installed benchmark guidance retains canonical `benchmark-report.md` only for dispatched workers, with no standalone baseline writes. Standalone destinations remain unchanged. Shared guidance adds no legacy recipe gate or archive mutation permission; real archive-consumer integration tests passed. |
| File classes, Store split, planning-only roots, handoff and sticky legacy | Resolver code is unchanged; file-placement tests passed. Shared guidance and orchestration distinguish required observations from disposable scratch and use CLI-resolved roots. Store selection remains in installed skills; no live Store was created. |
| Raw JSON, mutable fetched inputs, regenerable detail, source and legacy ephemera | Propose/explore and expert instructions preserve required originals once, identify availability, reference committed generators, and resolve required legacy-ephemera retention before cleanup. Existing verification-harness classification remains unchanged. |

## Availability and boundaries

The recipe fixture was an isolated disposable repository at commit `2d3191fa496657ed33000b0c75ea0118b2bb770a`; original synthetic input was 200 bytes with SHA-256 `5d4c38969111afb9caef4fbde7b1a391eb122927089ea102d02f42cb4550a46e`. Temporary source, installed skills, and data were removed after the smoke. This receipt records the check performed; that temporary commit is not a published reproduction dependency.

The MadoPilot archive and collectors, archive journal cost, generated relative-link defect, already-synchronized ADDED validation defect, existing archive bytes, and unrelated working-tree edits were not changed. No archive-performance improvement or storage-reduction measurement is claimed. The full test suite was not run locally; the Linux full suites and Windows shards ran in CI. Local verification targeted generation, installation, placement, workflow composition, archive consumers, and byte hygiene.
