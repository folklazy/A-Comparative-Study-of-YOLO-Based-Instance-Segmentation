# Integration scope

## What is included
- Per-frame person detection and instance segmentation (selected YOLO26x-Seg).
- Per-person human parsing (selected configuration to be verified).
- Upper/lower garment color extraction (selected method to be verified).
- Image/video ingestion and result overlays.
- API outputs, persistence and attribute-based retrieval.
- End-to-end quality and speed/resource evaluation with permission-cleared fixtures.
- Deployment, user documentation, versioned manifests and final academic evidence.

## Exclusions / boundaries
- Identity recognition or person identification.
- Tracking the same person across cameras.
- Unverified claims of general CCTV robustness or real-time throughput.
- Bulk copies of original research logs, unreleased checkpoints or company datasets.

## Functional acceptance test ideas
1. A frame with no people produces valid empty result.
2. Multiple people retain distinct instance masks and attribute records.
3. Crops and native-resolution masks align with original image coordinates.
4. Upper/lower clothing labels and colors are mapped consistently; missing regions become unknown.
5. Visualizations match stored API outputs and image dimensions.
6. API errors, bad input, unavailable GPU and missing checkpoint are handled.
7. Database search is deterministic for stored attributes.
8. Same frozen input/config yields reproducible outputs within supported numeric tolerance.
9. Image and video cases are both exercised.
10. Record errors in crowded/occluded/small/blurred/lighting-challenged frames, where permissions allow.

**No acceptance claim without actual test evidence.**
