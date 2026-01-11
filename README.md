# Cloud Cover Detection using DeepLabV3

This repository contains a **DeepLabV3-based semantic segmentation model** for **cloud cover detection in satellite imagery**. The model is trained using PyTorch and performs **pixel-level classification** to distinguish cloud and non-cloud regions.

The trained model weights (`.pth`) provided in this repository can be directly used for inference or further fine-tuning on custom geospatial datasets.

---

## Project Objective

Cloud cover significantly affects remote sensing and Earth observation analysis. This project aims to:

- Perform **binary semantic segmentation** of satellite images
- Generate accurate **cloud masks**
- Enable downstream tasks such as land-cover analysis, terrain monitoring, and change detection by masking clouds

---

## Repository Structure

```text
Cloud-Cover-DeepLabV3-Model/
│
├── final1_model1.pth          # Trained model (batch=1, epoch=15, input=256×256)
├── final1_model2.pth          # Trained model (batch=4, epoch=50, input=256×256)
├── final1_model3.pth          # Trained model (batch=8, epoch=35, input=256×256)
│
├── CloudDeeplabV3.ipynb       # Training and evaluation notebook
├── CloudDeeplabV3_v2.ipynb    # Alternative training configuration
│
├── training_results.csv       # Training and validation metrics
├── training_vs_validation_loss/
│   └── loss_plots.png         # Loss comparison plots
│
├── scripts/                   # Helper scripts (if applicable)
└── README.md
```
## Requirements

Ensure the following dependencies are installed:
`pip install torch torchvision numpy opencv-python matplotlib pillow tqdm`


