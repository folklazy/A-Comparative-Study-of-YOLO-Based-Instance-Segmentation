# Evidence index — release integrity

This is a navigation map, **not** evidence that the final runtime has already been assembled or tested.

| Area | Historical source | Items to pin before release |
|---|---|---|
| YOLO MOTS20 comparison | [Scaling Study](https://github.com/folklazy/YOLO_Instance_Segmentation_MOTS20_Scaling_Study) | chosen model, run settings, CSVs, hashes, qualitative cases |
| YOLO CCTV600 evaluation | [CCTV600 Scaling Study](https://github.com/folklazy/YOLO_Instance_Segmentation_CCTV600_Scaling_Study) | camera/condition subsets, actual evaluation splits and metrics |
| Human Parsing | [Parsing Study](https://github.com/folklazy/Human_Parsing_Study) | chosen model(s), taxonomy, masks, config, checkpoint hash |
| Human Parsing CCTV | [CCTV600 Benchmark](https://github.com/folklazy/Human_Parsing_CCTV600_Benchmark) | per-class scores and visual error evidence |
| Clothing color | [Garment Color Extractor](https://github.com/folklazy/Garment-Color-Extractor) | chosen extraction method, labels, matrices/prototypes, evaluation |
| CCTV GT | [Dataset Development](https://github.com/folklazy/CCTV_Dataset_Development) | counts, QA, split provenance, permissible publication metadata |
| Web + API + database | Private `folklazy/Body-Extraction-Human-WebApp` | code commit, database schema, API contract, deployment evidence |

## Fill when actual source was inspected

For each final component append:
- exact repository + source commit/tag;
- relevant path(s), selected configuration and reason;
- weight/checkpoint SHA256 and license/retrieval instruction;
- test report plus date and input denominator;
- whether figures are standalone benchmark, derived analysis or measured integrated behavior;
- data visibility classification.

Until then label information **UNVERIFIED**, never infer hashes or success rates.
