# Agent rules — final integrated Human Body Extraction

## Required reading
1. `README.md`
2. `docs/INTEGRATION_SCOPE.md`
3. `docs/RELEASE_CHECKLIST.md`
4. `docs/EVIDENCE_INDEX.md`
5. Relevant source repositories and their own AGENTS.md
6. `tasks/ACTIVE_TASK.md`, if present

## Authority / constraints
- This is the final deliverable, not an open-ended architecture experiment.
- The project owner reports implementation complete; first inspect the existing actual code, dataset rights, configs, model IDs and tests before migration.
- Import only reviewed/pinned components from YOLO, Parsing, Color, CCTV Dataset and Web Platform.
- Do not claim any model/configuration is selected beyond cited evidence. YOLO26x-Seg was selected in the prior YOLO study; the final parser/color model must be audited.
- Never edit or delete experimental archives, canonical metrics, trained weights, raw GT or raw CCTV footage without separate permission.
- Do not publish company imagery, annotation exports, identifying data, secrets, keys, connection strings or restricted checkpoints.
- Do not silently install dependencies, download large models, train/re-run benchmarks, rename classes, modify mask alignment or alter measured results.
- No deployment or push of sensitive files without audit and approval.
- Preserve source commit SHAs, dataset provenance, checkpoint hashes, licenses, config and environment.

## Engineering standards
- Create explicit component contracts with versioned schema and coordinate convention.
- Validate integration with unit, API, GPU/CPU (as applicable) and end-to-end smoke tests.
- Distinguish timing components; report actual end-to-end measurement rather than borrowed isolated benchmark speed.
- Keep a clean runnable installation guide only after verifying commands on the target machine.
- Handle uncertain color and unparseable persons as structured 'unknown', not fabricated confidence.

## Finish
- Record changed files, source SHAs, measured results, limits and reproduction logs.
- Update docs and CHANGELOG; complete release checklist with evidence.
- Remove `tasks/ACTIVE_TASK.md` only after verified completion and handoff. Never remove `AGENTS.md` or evidence files.
