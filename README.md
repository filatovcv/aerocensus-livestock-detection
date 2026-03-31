# AeroCensus Livestock Detection

An open-source AI/computer vision platform for automated detection and counting of livestock and wildlife from UAV (drone) aerial imagery. Initial data collection targets cattle on Texas ranches, with the goal of building models that generalize across U.S. cattle operations and transfer to wildlife census applications (white-tailed deer, feral hogs, other large mammals).

> **Status:** Pre-development. This repository is being set up as the foundation for a domain-specific benchmark study comparing multiple detection architectures on aerial livestock imagery. No trained models, datasets, or inference pipelines are available yet.

## Planned Scope

- **Multi-architecture benchmark** evaluating YOLO, Faster R-CNN, DETR/RT-DETR, EfficientDet, and SAM 2 on UAV-collected cattle imagery under real ranch conditions (variable altitude, lighting, terrain, herd density)
- **Annotated dataset** of RGB aerial images from Texas ranches, released under CC BY 4.0 (pending landowner consent), with transfer-learning support for adaptation to other U.S. regions
- **Training and inference pipelines** for reproducible model comparison
- **Edge deployment** configurations for drone-mounted hardware

## Motivation

The U.S. cattle inventory is 94.2 million head across 1.9 million operations (USDA Census of Agriculture, 2022). Accurate headcount documentation is a federal requirement under EPA CAFO regulations, USDA Animal Disease Traceability rules, and NASS survey methodology — yet current counting methods (manual ground surveys, operator self-reporting, manned aerial flights) remain expensive, infrequent, and error-prone.

Published CV research on aerial livestock detection consistently lacks publicly released model weights, annotated datasets, and deployable inference pipelines. This project aims to fill that gap.

## Planned Repository Structure

```
aerocensus-livestock-detection/
├── data/                # Dataset preparation and annotation tools
├── models/              # Architecture configs and training scripts
├── evaluation/          # Benchmark evaluation and comparison tools
├── inference/           # Inference pipelines and edge deployment
├── docs/                # Technical documentation
├── notebooks/           # Exploratory analysis and visualization
└── tests/               # Unit and integration tests
```

## Technical Stack (Planned)

Python · PyTorch · Ultralytics · Detectron2 · HuggingFace Transformers · OpenCV · CVAT (annotation)

## Author

**Nikolai Filatov** — M.S. Biology · 13 years software engineering · 5+ years AI/CV · 13 years government-certified wildlife census specialist, including aerial ungulate surveys

## License

**Code:** [Apache License 2.0](LICENSE)

**Dataset & model weights:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) *(will apply once released)*

## Citation

Citation information will be added once the first benchmark results are published.

---

*This README will be updated as development progresses.*
