# StreamingCoT

[![Dataset Access](https://img.shields.io/badge/Dataset-Anonymous%20Access-brightgreen)](https://anonymous.4open.science/)
[![Paper Status](https://img.shields.io/badge/Paper-Preprint-orange)]()

## Overview
StreamingCoT is the first large-scale dataset explicitly designed for temporally evolving reasoning in streaming Video Question Answering (VideoQA) and multimodal Chain-of-Thought (CoT) tasks. Addressing critical limitations in current VideoQA benchmarks, StreamingCoT features:

- **Dynamic temporal understanding**: Captures evolving answers in video streams
- **Explicit reasoning chains**: Provides annotated multimodal reasoning paths
- **Temporal dependency modeling**: Tracks semantic evolution across video timelines
- **Spatiotemporal grounding**: Links reasoning steps to visual evidence

This dataset establishes a new foundation for research in streaming video understanding, complex temporal reasoning, and multimodal inference.

## Key Features
### 🎥 Curated Video Corpus
- **5,745 high-quality short videos** (≤60 seconds)
- Global representation through stratified geographic sampling
- Rigorous multimodal filtering:
  - Social validation (>5,000 interactions)
  - Lexical density constraints
  - HD resolution (≥720p)
  - Motion dynamics analysis
  - Aesthetic scoring (≥7/10)

### ⏱️ Hierarchical Temporal Annotation
- **Per-second dense captions** aligned with visual content
- Adaptive temporal segmentation via Dynamic Semantic Fusion (DSF)
- Context-aware narration generation with inter-segment coherence
- Expert-validated semantic completeness and temporal alignment

### ❓ Dynamic QA Construction
- **6 specialized question types**:
  1. Cumulative counting
  2. Periodic pattern recognition
  3. Sequential step recognition
  4. State duration measurement
  5. Object state recognition
  6. Clue-revealing responses
- Distractor-aware option design targeting temporal misperceptions
- Human-verified temporal consistency and answer validity

### 🧠 Multimodal Chain-of-Thought
- **Spatiotemporally grounded reasoning chains**:
  1. Temporally-aware CoT initialization
  2. Key object extraction and spatial grounding
  3. Multimodal reasoning fusion
- Iterative human validation protocol ensuring:
  - Spatiotemporal consistency
  - Temporal causality
  - Evidence completeness
  - Answer derivation soundness

## Dataset Structure
```
StreamingCoT/
├── videos/                  # Original video files (MP4)
├── metadata/                # Video source and filtering info
├── annotations/
│   ├── dense_captions/      # Per-second and segment-level captions
│   ├── qa_pairs/            # Question-answer sets with options
│   ├── cot_chains/          # Multimodal reasoning chains
│   └── validation_reports/  # Human verification records
└── visual_grounding/
    ├── keyframes/           # Temporally significant frames
    └── bounding_boxes/      # Spatially grounded object annotations
```

## Construction Pipeline
Our hierarchical annotation framework:
1. **Video Collection & Filtering**  
   YouTube API → Geographic balancing → Multimodal quality screening
2. **Hierarchical Captioning**  
   Per-second captioning → Dynamic segmentation → Context-aware narration
3. **Dynamic QA Generation**  
   Question typing → Distractor design → Temporal realignment
4. **Multimodal CoT Synthesis**  
   Keyframe selection → Object grounding → Reasoning fusion
5. **Iterative Validation**  
   Expert verification → Error taxonomy → Corrective regeneration

## Applications
StreamingCoT enables research in:
- Temporal reasoning in video understanding
- Multimodal chain-of-thought development
- Streaming video question answering
- Spatiotemporally grounded inference
- Dynamic distractor analysis
- Video-based logical deduction systems

## Access
The StreamingCoT dataset and construction toolkit are available at:  
[https://anonymous.4open.science/](https://anonymous.4open.science/)

## License
StreamingCoT is released for non-commercial research purposes. All videos are sourced from YouTube and remain subject to original content creators' rights. Users must comply with YouTube's Terms of Service.

## Citation
```bibtex
@article{streamingcot2024,
  title={StreamingCoT: Advancing Temporal Reasoning in VideoQA through Dynamic Multimodal Chain-of-Thought},
  author={Anonymous},
  journal={Submitted to Preprint},
  year={2024},
  note={Dataset available at \url{https://anonymous.4open.science/}}
}
```

## Contact
For dataset inquiries, please open an issue on our repository or contact the maintainers through the anonymous submission portal.
