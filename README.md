# Polyp_segmentation_And_detection_Project
Final project in Medical Image Processing: Pixel-level segmentation and bounding-box detection of gastrointestinal polyps to aid clinical diagnostics.
## 👥 Team
* **Oren Chaushu**
* **Roni Hachinsky**

## 🎯 Project Overview
This project focuses on automating the detection and segmentation of polyps in endoscopic images using Deep Learning. Early detection is crucial for preventing colorectal cancer, and our model aims to assist medical professionals by providing robust, automated pixel-level segmentation.

## 📊 Dataset
We utilize the **Kvasir-SEG** dataset, which contains 1,000 annotated images of gastrointestinal polyps along with their corresponding ground-truth masks and bounding boxes.

## 🚀 How to Run the Code
This project is fully self-contained and designed to run easily in **Google Colab**.
1. Open the `Polyp_segmentation_&_detection_Project.ipynb` file directly in Google Colab.
2. **Data Access:** The dataset is accessed via a shared Google Drive folder. The notebook includes a cell that mounts Google Drive, allowing direct access to the data without requiring any manual local downloads by the reviewer.
3. Run the cells sequentially. The first cell will automatically install all required third-party libraries (e.g., `albumentations` and `torchmetrics`).

## 🛠️ Pipeline & Architecture
* **Framework:** PyTorch
* **Model Architecture:** U-Net (Medical Segmentation Baseline)
* **Data Augmentation:** Albumentations (Resizing to 256x256, Rotations, Flips, Gaussian Noise, Color Jitter)
* **Loss Function:** Dice Loss (implemented to address the extreme class imbalance between the background and the polyp)
* **Evaluation Metrics:** Intersection over Union (IoU) and Dice Coefficient
