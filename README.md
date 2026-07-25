readme = """# Automated Spinal MRI Analysis Using Deep Learning and brain MRI Analysis

## Project Overview
This project develops a deep learning framework for spinal MRI image preprocessing, enhancement, and classification of normal and pathological MRI scans.

## Features
- MRI preprocessing
- Image enhancement (CLAHE, Gaussian, Median filtering)
- Quality metrics (PSNR, SSIM, MSE, RMSE, UQI)
- EfficientNetB0 model
- Performance evaluation

## Dataset
- 10 Normal Spine MRI patients
- 10 Pathological Spine MRI patients
- NIfTI (.nii.gz) format

## Requirements
See requirements.txt

## How to Run
1. Enable GPU.
2. Run all notebook cells.
3. The trained model will be saved as `spinal_mri_model.keras`.

## Results
- Image enhancement completed
- Model trained and evaluated
"""

with open("README.md", "w") as f:
    f.write(readme)

print("README.md created successfully!")

# Brain MRI Enhancement and ROI Segmentation using U-Net

## Overview

This project presents an AI-based framework for Brain MRI enhancement and Region of Interest (ROI) segmentation using Deep Learning. MRI images are first enhanced through preprocessing techniques and then segmented using the U-Net architecture to detect lesion regions.

The system is designed to assist radiologists by providing accurate and automatic lesion segmentation from Brain MRI scans.

---

## Features

- Brain MRI Dataset Analysis
- MRI Image Preprocessing
- Image Quality Evaluation
- ROI Segmentation using U-Net
- Prediction Visualization
- Streamlit-based User Interface

---

## Dataset

Dataset Used:

- BraTS 2020 Brain MRI Dataset

MRI Modalities:

- T1
- T2
- T1CE
- FLAIR

Ground Truth segmentation masks are used for supervised learning.

---

## Project Workflow

### Stage 1: Dataset Analysis

- Load MRI dataset
- Visualize MRI slices
- Patient-wise analysis
- Mask visualization

---

### Stage 2: MRI Enhancement

Preprocessing includes:

- Image resizing (128×128)
- Intensity normalization
- Slice extraction
- Noise reduction

Quality Metrics:

- Contrast
- Brightness
- Sharpness
- Noise Estimation
- Edge Strength

---

### Stage 3: ROI Segmentation

Deep Learning Model:

- U-Net

Training Configuration:

- Optimizer: Adam
- Learning Rate: 0.0001
- Loss Function: Binary Cross Entropy
- Batch Size: 8
- Epochs: 5

---

## Model Performance

Validation Accuracy: **97.71%**

Validation Loss: **0.0553**

Training Loss: **0.0598**

The model successfully detects lesion regions in Brain MRI images.

---

## Technologies Used

- Python
- TensorFlow
- Keras
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Scikit-image
- SciPy
- Streamlit
- Pillow
- Nibabel

---

## Folder Structure

Brain_MRI_Project/

│── app.py

│── brain_roi_unet_final.h5

│── notebook.ipynb

│── README.md

│── requirements.txt

│── training_history.csv

│── sample_images/

│── predicted_results/

---

## Installation

Clone the repository:

```bash
git clone <repository-link>
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Run the Application

```bash
streamlit run app.py
```

---

## Output

The application provides:

- MRI Upload
- Enhanced MRI
- ROI Prediction
- Segmentation Mask
- ROI Overlay

---

## Future Improvements

- Spine MRI Segmentation
- Multi-class Segmentation
- Attention U-Net
- 3D U-Net
- MONAI Framework
- Clinical Deployment

---

## Authors

Kruthi N

Devika

Department of Information Science & Engineering

NMAM Institute of Technology, Nitte

---

## License

This project is developed for academic and hackathon purposes.
