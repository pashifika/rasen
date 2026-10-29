## Why

Evidence packages become expensive to archive and review when reproducible outputs duplicate their inputs and historical observations are treated like disposable logs. Rasen should help users retain decisions and irreplaceable observations while replacing regenerable detail with pinned generator source, identified inputs, and explicit reproduction instructions.

## What Changes

- Teach one source-backed evidence contract across generated planning, investigation, benchmark, verification, and delivery guidance: distinguish deterministic regeneration, reanalysis of retained observations, and a fresh experimental rerun.
- Keep a compact current decision record and one reproduction recipe per evidence scope. Reuse an existing canonical report or index rather than requiring another report hierarchy.
- Identify generator and measured-source repositories and commits, actual source deviations, inputs, relevant dependencies/environment, commands, expected outputs, and availability. A commit alone is not proof of a past result or sufficient identification of a dirty execution.
- Replace duplicated deterministic fixtures and derived detail with recipes and references when regeneration has been demonstrated. Preserve the minimum observation set needed to audit a historical claim, including failed and incomplete outcomes.
- Clarify the existing seven-class placement guidance so retention depends on a file's use and lifecycle, not on its being JSON, stdout, or a raw capture. Preserve existing placement roots, standalone behavior, Store selection, and sticky-legacy handling.
- Keep summaries bounded by decisions and evidence references rather than by the number of samples. Establish the intended claim and stopping condition before a collection campaign; this does not reduce required statistical samples or verification gates.

## Capabilities

### New Capabilities

- `source-backed-evidence-retention`: User-visible workflow guidance for compact evidence, pinned reproduction recipes, retained historical observations, and truthful availability/reproducibility claims.

### Modified Capabilities

- `file-placement`: Clarify how irreproducible observation evidence differs from disposable collection output and regenerable intermediates, without adding a file class or changing archive-engine disposition semantics.

## Impact

- Generated workflow/expert instructions under `src/core/templates/`, their existing shared guidance, delivered skill documentation, and user-facing documentation of evidence handling.
- File-placement documentation and comments; existing canonical report names and machine-readable verdict/test-evidence fields stay compatible.
- Implementation verification must exercise actual generated/installed guidance and a small disposable evidence example. No new CLI command, dependency, automatic execution service, storage backend, or retention configuration is proposed.
- Existing archives, journals, hashes, Git ignore policies, and raw observations remain unchanged. Missing legacy recipes are not retroactive delivery blockers.
- Archive journal checkpoint optimization and canonical-spec relative-link rebasing are separate changes. MadoPilot collector changes, historical archive compaction, data relocation/deletion, and a new performance campaign are outside this Change.
