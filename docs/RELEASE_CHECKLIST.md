# Final release checklist

## 0. Provenance
- [ ] Confirm selected model, weights, checkpoint SHA256 and license for each module.
- [ ] Record audited Git source commits and config hashes.
- [ ] Confirm dataset/fixture rights and prevent public disclosure.

## 1. Packaging
- [ ] Separate runtime code, configurations, tests, demo-safe assets, user documentation.
- [ ] Lock Python/JS dependencies and supported driver/CUDA hardware.
- [ ] Provide reproducible installation, configuration and startup commands.
- [ ] No absolute personal home paths, API keys, secrets or large generated files.

## 2. Integration
- [ ] Version and validate module interfaces and parser/color taxonomy mappings.
- [ ] Validate native image and mask dimensions.
- [ ] Test no-person, one-person, multiple-person, overlap, bad input, failure recovery.
- [ ] Verify image and video mode and database persistence/search.

## 3. Evaluation
- [ ] Keep isolated benchmark accuracy/speed distinct from end-to-end outcomes.
- [ ] Report actual end-to-end FPS/latency/VRAM on identified hardware and sample set.
- [ ] Collect visual success/failure examples with sharing permission.
- [ ] Document scope, limitations, sample counts and confidence/unknown rules.

## 4. Delivery
- [ ] README, installation, API, database, deployment, user manual and research evidence index.
- [ ] Check git history, links, license notices and data privacy.
- [ ] Mark release/tag only when all required gates have documented evidence.
- [ ] Record owner acceptance and final handoff summary.
