readme = """# Automated Spinal MRI Analysis Using Deep Learning

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
