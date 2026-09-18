# BCDD-SUST: An Annotated Peripheral Blood Cell Dataset for AI-Based Dengue Diagnosis

## Overview

BCDD-SUST (Blood Cell Dataset of Dengue - SUST) is an expert-validated peripheral blood smear image dataset developed for research on blood-cell detection, classification, digital hematology, computer vision, and AI-based dengue research.

The dataset contains 5,692 peripheral blood smear images collected from 50 patient samples, including 25 dengue NS1-positive and 25 dengue NS1-negative samples. The dataset provides 50,966 expert-validated bounding-box annotations covering seven blood-cell classes:

- Band Neutrophil
- Giant Platelet
- Monocyte
- Normal Lymphocyte
- Platelet
- Reactive Lymphocyte
- Segmented Neutrophil

All images are annotated in YOLO format and organized into training, validation, and test sets.

## Directory Structure

```
BCDD-SUST/
├── train/
│   ├── images/
│   └── labels/
├── valid/
│   ├── images/
│   └── labels/
├── test/
│   ├── images/
│   └── labels/
├── data.yaml
├── manual_annotation_protocol.pdf
├── image_metadata.xlsx
└── metadata.xlsx
```

- `images/`: Contains all images, split into train/val/test.
- `labels/`: YOLO-format annotation files, split into train/val/test.
- `data.yaml`: YOLO dataset configuration file.
- `manual_annotation_protocol.pdf`: Manual annotation and quality-control protocol.
- `image_metadata.xlsx`: Contains per-image cell count data
- `metadata.xlsx`: Clinical and demographic data  mapped to slide samples

## Usage

The dataset can be used directly with object-detection frameworks supporting the YOLO annotation format.

Potential applications include:

- Blood-cell detection and classification
- Digital hematology analysis
- AI-based dengue research

## License

This dataset is licensed under the MIT License.
