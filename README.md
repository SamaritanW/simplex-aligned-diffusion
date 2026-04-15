# Simplex-Aligned Diffusion with Cross-Granularity Interaction for Robust Medical Image Classification

[![MIDL 2026](https://img.shields.io/badge/MIDL-2026-blue)]()
[![Paper](https://img.shields.io/badge/OpenReview-Paper-green)](https://openreview.net/forum?id=BoKB1aGqRn#discussion)

Official PyTorch implementation of the MIDL 2026 paper:

**Simplex-Aligned Diffusion with Cross-Granularity Interaction for Robust Medical Image Classification**


## Abstract

Standard diffusion models apply Gaussian noise directly to one-hot classification labels on the probability simplex, causing probability leakage and mathematical inconsistency. We propose Simplex-Aligned Diffusion, which performs diffusion in an unconstrained logit space via Centered Log-Ratio (CLR) mapping, ensuring rigorous geometric consistency throughout the diffusion process. Combined with a Cross-Granularity Interaction module that captures multi-scale semantic features, our method achieves reliable uncertainty quantification and robust calibration under clinical noise conditions.

## Key Contributions

- **Simplex-Aligned Diffusion**: Resolves the bounded vs. unbounded conflict by mapping labels to logit space before diffusion, eliminating probability leakage
- **Cross-Granularity Interaction**: Enables feature interaction across multiple scales for improved robustness to noise
- **Robust Calibration**: Maintains reliable uncertainty estimates under continuous clinical noise (defocus, motion) across varying severity levels

## Results

Evaluated on HAM10000 and APTOS2019 datasets under multiple noise types and severities. Our method consistently outperforms DiffMIC-v2 on accuracy, F1, Cohen's Kappa, and Expected Calibration Error (ECE).

## Code

Code coming soon. Please star this repo to get notified.

## Citation

If you find this work useful, please cite:

## Citation

If you find this work useful, please cite:

```bibtex
@inproceedings{wusimplex,
  title={Simplex-Aligned Diffusion with Cross-Granularity Interaction for Robust Medical Image Classification},
  author={Wu, Chao and Gao, Mingchen},
  booktitle={Medical Imaging with Deep Learning}
}
```
