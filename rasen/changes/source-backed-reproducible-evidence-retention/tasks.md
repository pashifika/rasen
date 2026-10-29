## 1. Shared evidence contract

- [ ] 1.1 Add the shared evidence-retention template module and explicit integration list described in design Decision 1. Cover deterministic regeneration, historical reanalysis, experimental reruns, and the distinction between a recipe and an observed outcome.
- [ ] 1.2 Define the compact report/index recipe guidance: claim and stopping condition, generator and measured-source identities, dirty/untracked deviations, inputs and availability, command/base, relevant environment, expected result domain, and performed checks. Preserve existing machine-readable report fields and avoid a new mandatory sidecar format.
- [ ] 1.3 Reconcile the shared guidance with `src/core/file-placement.ts` documentation and existing probe-placement guidance: required original observations remain evidence, reproducible detail is ephemera, and committed generators are referenced without source duplication. Keep existing classes, resolved roots, and sticky-legacy behavior.

## 2. Producer and consumer integration

- [ ] 2.1 Integrate the contract into planning and implementation/orchestration templates, including propose/explore research handling and orchestration-embedded skills. Teach claim-first collection and one authoritative recipe without duplicating guidance inside an emitted skill.
- [ ] 2.2 Integrate the contract into the expert shared preamble and reconcile investigation/benchmark collection and reporting instructions. Preserve standalone destinations and dispatched canonical-report-only restrictions; distinguish retained observations from disposable detailed reports and scratch output.
- [ ] 2.3 Integrate verification and review-cycle guidance so readers can assess source/input availability and historical claims without automatically executing recipes. Preserve canonical verdicts and test-evidence consumption.
- [ ] 2.4 Reconcile ship, single/bulk archive, and retention guidance with source-backed evidence references. Preserve existing gates, exact-token recovery/ownership rules, archive immutability, and legacy reports without recipes; do not introduce automatic cleanup or a new archive blocker.

## 3. Verification of delivered behavior

- [ ] 3.1 Use the existing workflow-generation/skill-installation checks to verify affected generated artifacts remain installable and retain consumer-visible report contracts. Update behavioral coverage only where a plausible regression needs it; remove affected incidental wording/hash assertions rather than re-pinning them as correctness evidence.
- [ ] 3.2 Build the CLI and generate/install affected skills into an isolated temporary project using the normal product path. Inspect the actual emitted planning, benchmark, verification, and archive instructions for consistent mode/retention guidance, preserved Store selection, and dispatched/standalone restrictions.
- [ ] 3.3 Exercise a disposable deterministic generator with pinned source and inputs, verify its expected digest, and derive a compact decision plus reproducible detailed report from a small retained observation dataset. Confirm the same declared aggregates/verdict can be recreated without duplicating the observation array in the summary.
- [ ] 3.4 Exercise the evidence scenarios for changed or missing inputs, private originals, dirty source, variable output metadata, and a new timing run. Confirm unavailable/unverified reproduction stays explicit, new observations do not rewrite historical outcomes, and report inspection does not itself execute commands.
- [ ] 3.5 Verify path-aware generation and recipe examples with spaces and explicit repository bases on supported platforms. Run the affected Windows CI job and record its result separately from local macOS/Linux checks; do not treat POSIX-only observation as Windows verification.
- [ ] 3.6 Run the affected generation/installation and downstream report-consumer checks after implementation, plus type checking and lint. Select any broader suite from actual cross-cutting risk; use `env -u ZSH pnpm test` if the full suite is required. Record only exercised results and remove disposable smoke outputs.

## 4. Documentation and delivery evidence

- [ ] 4.1 Update the existing user-facing file-placement/workflow documentation and release changelog with the source-backed retention contract, compact recipe example, historical-observation limits, and unchanged archive/Git boundaries. Keep shipped skill documentation consistent with its template source through the existing generation route.
- [ ] 4.2 Record a compact verification report mapping the new capability and file-placement scenarios to the actual delivered guidance and smoke results. Leave all historical archives and both separately reported archive defects unchanged; do not claim archive performance gains or MadoPilot collector changes.
