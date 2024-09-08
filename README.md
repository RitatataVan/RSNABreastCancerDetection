# RSNA Screening Mammography Breast Cancer Detection

![breastcancer](https://github.com/user-attachments/assets/1300499d-2c2b-4a6a-a91a-253333d1976c)

## Background
The aim is to identify breast cancer. We trained model with screening mammograms obtained from regular screening. The work improving the automation of detection in screening mammography may enable radiologists to be more accurate and efficient, improving the quality and safety of patient care. It could also help reduce costs and unnecessary medical procedures.

## Challenges
- Image (Dicom) preprocessing
- Data imbalance issues

## Data
Dataset: https://www.kaggle.com/competitions/rsna-breast-cancer-detection/data <br>
Extra Dataset: https://www.kaggle.com/datasets/pourchot/ddsm-mammography-positive-case

## Preprocess

## Methods
- Conducted VOI-LUT to adjust grayscale, used YOLOX-m for ROI Cropping, and resized images to a 1.75:1 aspect ratio with padding for data pre-processing
- Implemented undersampling by choosing a smaller subset of the majority class to address imbalanced data issue
- Employed ConvNextV2Tiny with a global average pooling layer for binary classification of breast cancer detection, achieving superior pF1 scores
