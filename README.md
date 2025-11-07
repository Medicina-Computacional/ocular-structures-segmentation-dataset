# Annotated Dataset for Retinal Fundus Image Segmentation: Vascular Arcade and Optic Nerve

## Overview

This dataset provides annotated masks for retinal fundus images, focusing on two critical ophthalmic structures: the vascular arcade and the optic nerve. The dataset consists of 500 fundus images sourced from the [Asia Pacific Tele-Ophthalmology Society 2019 Blindness Detection (APTOS 2019 BD)](https://www.kaggle.com/competitions/aptos2019-blindness-detection) dataset. Each image is accompanied by segmentation masks, representing the vascular arcade and optic nerve, to facilitate the development and evaluation of segmentation models in computational ophthalmology.

This dataset is valuable for training, benchmarking, and fine-tuning segmentation algorithms for the analysis of retinal images, particularly in the context of diabetic retinopathy and other ophthalmic conditions.

---

## Data Description

The dataset consists of:

- **500 fundus images:** Sourced from the APTOS 2019 BD dataset, available on Kaggle.
- **Masks in PNG format:** Representing the vascular arcade (1), optic nerve (2), and background (0).
- **Annotations:** Provided in COCO 1.0 format (JSON), which can be used to generate the corresponding masks.
- **Resolution:** The images have varying resolutions, ranging from 474×358 pixels to 4288×2848 pixels.

---

## Example Visualizations

Example corresponding masks (highlighting the vascular arcade and optic nerve) are included in the dataset for reference.

---

## Data Collection

- **Source of Fundus Images:** [APTOS 2019 Blindness Detection dataset](https://www.kaggle.com/competitions/aptos2019-blindness-detection)
- **Data Annotations:** Generated at the **Universidad Autónoma de Baja California (UABC)** using the **Computer Vision Annotation Tool (CVAT)**.
- **Mask Formats:**  
  - 0: Background  
  - 1: Vascular Arcade  
  - 2: Optic Nerve

---

## Value of the Data

- **Training & Benchmarking:** The dataset provides manual annotations of critical ophthalmic structures, which can be used for training AI models, parameter tuning, and benchmarking against human performance.  
- **AI Model Development:** Useful for developing robust and specialized algorithms for ophthalmic image segmentation.

---

## License

This dataset is released under the **Apache 2.0 License**, allowing researchers and developers to freely use, modify, and distribute the data.

---

## Usage

### Usage Instructions

#### 1. Download the Data

Clone or download the repository, which includes the 500 pre-generated masks in PNG format, ready for use in segmentation tasks. These masks correspond to the vascular arcade and optic nerve annotations.

Additionally, the `annotations_COCO.json` file is included, which contains the COCO format annotations.

#### 2. Prepare the Paths

Set the path to the annotations file in your script:

```python
annotations_path = 'path/to/annotations_COCO.json'
