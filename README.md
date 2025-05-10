[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15381211.svg)](https://doi.org/10.5281/zenodo.15381211)

# AI-Based Inference of Subsurface Structures from SAR Data

## Overview
This repository presents an open-source framework for detecting underground voids and material anomalies using machine learning models trained on synthetic and real Synthetic Aperture Radar (SAR) data. The intended application is archaeological exploration—non-invasive, remote sensing of ancient and potentially fragile subsurface environments.

## License
**Creative Commons CC0 1.0 Universal (Public Domain Dedication)** — This work is freely available for use, modification, and commercial or non-commercial redistribution in any domain.

## Summary
Recent advances in SAR resolution and AI-driven pattern recognition enable new tools for exploring underground spaces. This project documents a learning-based approach that infers 3D subsurface structure maps from 2D SAR imagery, without requiring explicit physical modeling or geophysical simulation. While developed with archaeological use in mind, the method itself is general.

## Core Method
- **Input**: High-resolution SAR data (complex-valued: phase + amplitude), ideally in spotlight or staring mode.
- **Training Data**:
  - Synthetic SAR simulations over parametrically generated void and cavity structures.
  - Real SAR paired with validated 3D subsurface models for supervised learning.
- **Neural Architecture**:
  - Deep learning models (CNNs, UNets, transformers) trained to predict volumetric probability maps of subterranean structure.
- **Domain Adaptation**:
  - Use of transfer learning, style-matching, or contrastive loss to generalize from synthetic to real environments.

## Intended Use Cases
- Identification of buried chambers, tunnels, or walls in heritage zones.
- Remote triage of sites for potential excavation.
- Complement to other passive or non-invasive scanning tools (e.g., LIDAR, magnetic).

## Technical Distinction
This approach uses **data-driven inference**, not physical or resonance-based inversion. It infers relationships directly from empirical patterns in surface radar response, via supervised training.

## Roadmap
- [ ] Upload baseline synthetic dataset generator
- [ ] Release pre-trained demo model for sample terrain
- [ ] Add 3D visualization interface (e.g., VTK or Three.js)
- [ ] Enable real-time SAR tile inference

## Diagram
See `images/pipeline.png`.

## Citation Guidance
While not required, citation is appreciated if used in academic or derivative work.

## Acknowledgment of Landscape
This implementation represents one possible path toward non-invasive SAR-based subsurface mapping. It is distinct from analytic or physics-modeled approaches, and offered here to broaden exploratory and collaborative research potential.

