# CFRP Defect Detection Using YOLOv5 and Thermal Image Enhancement

This repository demonstrates a machine learning pipeline to detect subsurface defects in Carbon Fibre-Reinforced Polymer (CFRP) composites using thermal video frames processed with signal-to-noise ratio (SNR) enhancement techniques and YOLOv5 object detection.

## Project Structure

```
cfrp-defect-detection-yolov5/
├── model/                               # Final trained YOLOv5 model and weights
├── Preprocessing scripts/               # CLAHE, Bilateral, Sobel Operator-Based Gradient Subtraction preprocessing scripts
├── Preprocessing results/               # Evaluation PDFs, output images, and visualisations
├── YOLO Training Script/                # YOLOv5 training and prediction notebooks/scripts
├── README.md                            # Project overview and instructions
├── requirements.txt                     # Python dependencies
└── .gitignore                           # Exclusions for GitHub
```

## Overview

- **Dataset**: 480 thermal frames (not publicly available), generated via Eddy Current Pulse-Compression Thermography (ECPuCT) [Yi et al., 2019].
- **Preprocessing**: CLAHE, bilateral filtering, and Sobel operator-based gradient subtraction to improve visibility and SNR.
- **Model**: YOLOv5m fine-tuned on annotated thermal image dataset.
- **Evaluation**: Precision, Recall, mAP scores; SNR impact reported via structured PDF evaluations.


## Included Evaluation Files

Located in the `Preprocessing results/` folder:
- `Gradient_snr_analysis.pdf`
- `CLAHE_snr_analysis.pdf`
- `Bilateral_snr_analysis.pdf`
- `SNR analysis script`

## Citation

> Sharma, Niranjan. "Enhancing Defect Detection in Carbon Fibre-Reinforced Polymers Using YOLOv5 and Thermal Image Preprocessing." BSc Dissertation, Northumbria University, Newcastle Upon Tyne, UK, 2025.
> Yi, Q., Tian, G.Y., Malekmohammadi, H., Zhu, J., Laureti, S. and Ricci, M., 2019. New features for
delamination depth evaluation in carbon Fibre reinforced plastic materials using eddy current
pulsecompression thermography. NDT & E International, 102, pp.264-273.

## Contact

Niranjan Sharma: niranjan.sh18@gmail.com

**Note**: The dataset is private. This repo shares reproducible methods, metrics, and evaluation reports only.
