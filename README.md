# A Comparative Study of YOLO-Based Instance Segmentation
## Final End-to-End Human Body Extraction for CCTV

This repository is the **final product and academic delivery**. It is separate from experimental archives and the coordination hub.

> **Current repository status: delivery packaging / audit.** The project owner reports that implementation and experiments are complete. The actual deployable module snapshot, lockfiles, checkpoint manifest and end-to-end reproduction steps still require verification before this README can claim a reproducible release.

## Intended end-to-end system

1. **Input:** CCTV images or videos.
2. **YOLO Person Instance Segmentation:** detect persons and return individual masks; selected candidate from prior comparative testing: **YOLO26x-Seg**.
3. **Human Parsing:** classify body/clothing regions for each person using the actually selected parser configuration.
4. **Clothing Color Extraction:** classify upper and lower garment colors, including uncertain or multi-color cases as supported by the selected method.
5. **Structured Results:** person-local masks, garment part labels and colors with confidence/unknown handling where supported.
6. **Web Application + API + Database:** image/video processing, visual overlays, saved results and attribute-based retrospective search.
7. **Final Evaluation:** integration correctness, visual error analysis, throughput/VRAM, limitations and safe sample outputs.

This system is **not** intended for identity verification or cross-camera identity tracking.

## Source of truth / related repositories

- [Project Hub](https://github.com/folklazy/Human-Body-Extraction)
- [YOLO MOTS20 Scaling Study](https://github.com/folklazy/YOLO_Instance_Segmentation_MOTS20_Scaling_Study)
- [YOLO CCTV600 Scaling Study](https://github.com/folklazy/YOLO_Instance_Segmentation_CCTV600_Scaling_Study)
- [Human Parsing Study](https://github.com/folklazy/Human_Parsing_Study)
- [Human Parsing CCTV600 Benchmark](https://github.com/folklazy/Human_Parsing_CCTV600_Benchmark)
- [Garment Color Extractor](https://github.com/folklazy/Garment-Color-Extractor)
- [CCTV Dataset Development](https://github.com/folklazy/CCTV_Dataset_Development)
- Existing private web implementation: `Body-Extraction-Human-WebApp`.

Do **not** treat links as evidence that code has already been migrated or a release has passed tests. Check [Evidence Index](docs/EVIDENCE_INDEX.md).

## Release gate

Before declaring this repo deployable:
- [ ] Audit actual selected model versions, code commits, checkpoint licenses and SHA256 hashes.
- [ ] Confirm current frontend/backend/database structure and pin dependencies.
- [ ] Integrate only vetted code; preserve upstream repo history and separate experiment artifacts.
- [ ] Define versioned input/output JSON contracts including coordinate systems and unknown attributes.
- [ ] Test the actual end-to-end pipeline on permission-cleared example media.
- [ ] Measure integrated timing and VRAM; differentiate these from isolated benchmark figures.
- [ ] Prepare install/deploy/user/API guides without publishing company CCTV data or secrets.

See [AGENTS.md](AGENTS.md), [Integration scope](docs/INTEGRATION_SCOPE.md) and [Release checklist](docs/RELEASE_CHECKLIST.md).
