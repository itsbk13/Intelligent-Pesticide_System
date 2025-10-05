# Models Directory

This directory contains trained models and associated configuration files for the Intelligent Pesticide System project.

## Contents

- `trained/`: Pretrained and fine-tuned model checkpoint files (.pth) for different architectures:
  - `UNet-ResNet50_trained.pth`
  - `UNet-EfficientNet_trained.pth`
  - `DeepLabV3Plus-ResNet50_trained.pth`
  - `DeepLabV3Plus-EfficientNet_trained.pth`
  - `NWRD-ResNet50_trained.pth`
  - `NWRD-EfficientNet_trained.pth`
 
## Usage of NWRD Model

The NUST Wheat Rust Disease (NWRD) pretrained models included in this project to train alongside **PlantSeg** dataset for high-precision leaf segmentation. Subsequently, these models are fine-tuned and integrated with the **DiaMOS** dataset to perform disease severity classification across four categories: Healthy, Mild, Moderate, and Severe.

This multi-stage training approach leverages the high-quality segmentation masks of PlantSeg to improve feature extraction, while the diverse and challenging classifications from DiaMOS enable accurate severity prediction.

For more details on the original NWRD research, visit the [NUST Wheat Rust Disease Project](https://github.com/dll-ncai/NUST-Wheat-Rust-Disease-NWRD).


## Important Notes

- The model checkpoint files are **large** (up to 124.4 MB each) due to the complexity and size of the networks.

- These files are necessary to reproduce the evaluation results and run inference demos.

## Usage

- Load these `.pth` files using the provided model loading via the notebooks.

- Ensure dependencies as defined in `requirements.txt` are installed for smooth model integration.

---

*For more information on model training and architecture, please refer to [05_training_pipeline](05_training_pipeline.ipynb) and [04_model_architecture](04_model_architecture.ipynb)*
