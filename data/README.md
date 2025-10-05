# Data Directory

This directory contains metadata and processed data files required for the Intelligent Pesticide System project.

## Contents

- `metadata/`: Contains CSV and JSON files describing datasets, including annotations, sample counts, and integrated dataset statistics.
  - Includes:
    - `plantseg_metadata.csv`
    - `diamos_metadata.csv`
    - `integrated_train.csv`, `integrated_val.csv`, `integrated_test.csv`
    - Dataset summaries and analyses (`dataset_info`, `dataset_summary.json`)

- **Note:** The `raw/` directory containing the original PlantSeg and DiaMOS datasets is **NOT included** in this repository due to data size and licensing restrictions.

## About the Raw Data (PlantSeg and DiaMOS)

- **PlantSeg Dataset:** A large collection of high-resolution microscopy images with pixel-wise segmentation masks for leaves.

- **DiaMOS Dataset:** A comprehensive set of images annotated with wheat rust disease severity levels across four severity classes: Healthy, Mild, Moderate, Severe.

- **Integration:** Data from PlantSeg and NWRD are combined and processed to form a unified dataset for training and evaluation.

## Obtaining the Raw Data

To obtain the raw PlantSeg and DiaMOS data, please refer to their respective official sources:

- PlantSeg: [Reference](https://www.kaggle.com/datasets/weitianqi/plantseg)
- DiaMOS: [Reference](https://www.kaggle.com/datasets/alexandraneagu101/diamos-plant-dataset)

## Usage

The metadata files and integrated datasets in this directory are used to:

- Provide training, validation, and test splits
- Supply class distributions and severity annotations
- Facilitate dataset statistics and analysis
