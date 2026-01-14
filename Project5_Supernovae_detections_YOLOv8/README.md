# Supernova Detection in Pan-STARRS Images using YOLOv8

## Overview
This project investigates the use of modern object detection techniques for identifying **supernova candidates** in astronomical survey images. Using imaging data from the **Pan-STARRS survey**, the task of supernova detection is framed as an **object detection problem**, where transient sources are localized within telescope images.

A **YOLOv8-based deep learning model** is trained and evaluated to detect supernovae against complex astronomical backgrounds, demonstrating the applicability of computer vision methods to time-domain astronomy.

---

## Scientific Motivation
Supernovae are transient astrophysical events that play a critical role in understanding stellar evolution, nucleosynthesis, and cosmology. Large sky surveys such as Pan-STARRS generate vast amounts of imaging data, making automated and scalable detection methods essential.

This project explores whether a data-driven object detection pipeline can assist in identifying supernova candidates efficiently, complementing traditional astronomical detection techniques.

---

## Dataset
The dataset used in this project is sourced from **Harvard Dataverse** and contains labeled Pan-STARRS astronomical images suitable for object detection tasks.

**Dataset DOI:**  
https://doi.org/10.7910/DVN/JGO6VI

The dataset includes:
- Astronomical images from the Pan-STARRS survey  
- Bounding box annotations for supernova candidates  
- A dataset configuration file compatible with YOLO-style training  

---

## Methodology
The workflow implemented in this project includes:

1. **Data Inspection and Visualization**
   - Verification of image integrity and structure  
   - Visualization of astronomical features and labeled regions  

2. **Dataset Preparation**
   - Exploration of directory structure and annotation formats  
   - Validation of dataset configuration for YOLO training  

3. **Model Training**
   - Training a YOLOv8 object detection model on Pan-STARRS images  
   - Leveraging transfer learning for stable convergence  

4. **Model Evaluation**
   - Validation of detection performance on held-out data  
   - Analysis of predicted bounding boxes and confidence scores  

All experiments are conducted using **Python**, with standard scientific and deep learning libraries.

---

## Tools and Libraries
- Python  
- Ultralytics YOLOv8  
- NumPy  
- OpenCV  
- Matplotlib  

Training and evaluation were performed in a GPU-enabled environment.

---

## Results
The trained model demonstrates the ability to localize supernova candidates in astronomical images, highlighting the potential of object detection frameworks for transient detection in large-scale sky surveys.

This work serves as a proof of concept for integrating modern computer vision pipelines into observational astronomy workflows.

---

## File Description
- `supernova-detections.ipynb` — Jupyter Notebook containing data exploration, model training, and evaluation steps  

---

## Future Work
- Extension to multi-epoch temporal modeling  
- Reduction of false positives through post-processing or ensemble methods  
- Application to additional transient classes (e.g., variable stars, AGN flares)  

---

## Acknowledgements
- Pan-STARRS Survey  
- Harvard Dataverse  
- Ultralytics YOLOv8 framework  
