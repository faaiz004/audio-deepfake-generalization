# Audio Deepfake Domain Generalization

Evaluate whether audio deepfake detectors generalize to unseen speech generators using **RawNet2**, **MLAAD**, and **M-AILABS**.

## Experiments

- Compare **ERM, IRM, CORAL, and GroupDRO** on French speech.
- Train on four synthesis generators and test on two unseen generators across four selected splits.
- Keep utterances disjoint across training, validation, and testing.
- Evaluate accuracy and Equal Error Rate (EER), with UMAP visualizations of learned representations.

## Results

Mean per-domain EER across the held-out evaluations:

| Method | EER ↓ |
|--------|-------|
| ERM | 35.01% |
| IRM | 35.55% |
| CORAL | 33.74% |
| GroupDRO | **33.35%** |

