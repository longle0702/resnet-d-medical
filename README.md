
# ResNet-D Medical Image Classification

This repository contains the research and code for implementing the ResNet-D architecture for medical image classification, specifically aimed at diagnosing lung diseases from X-ray scans. Our study focuses on optimizing the ResNet-D model to accurately classify medical images, highlighting enhancements in feature extraction and model accuracy through advanced training techniques and data augmentation.

## Team Members
- Nguyen Quang Huy - 22BI13195
- Nguyen Tuan Khai - 22BI13202
- Nguyen Hai Dang - 22BI13073
- Le Linh Long - 22BI13262
- Pham Thai Son - 22BI13397

## Project Overview

Medical image classification plays a crucial role in healthcare, aiding in early disease detection and diagnosis. This project leverages the ResNet-D architecture for classifying lung conditions based on X-ray scans. By incorporating advanced training methodologies and data augmentation, the model demonstrates improved accuracy and robustness.

### Key Features
- **ResNet-D Architecture**: Based on the ResNet family, ResNet-D utilizes an average pooling layer to reduce information loss, especially in downsampling.
- **Learning Rate Optimization**: Implements Learning Rate warm-up and Cosine Learning Rate Decay to stabilize and improve model training.
- **Data Augmentation**: Techniques such as random rotation, color inversion, and Gaussian blur address class imbalances and enhance model generalization.

## Dataset

The model uses the [COVID-19 Radiography Dataset](https://www.kaggle.com/datasets/preetviradiya/covid19-radiography-dataset), which includes X-ray images for:
- COVID-19 positive cases
- Normal cases
- Viral Pneumonia cases
- Lung Opacity cases

## Repository Structure

```
├── data/                  # Dataset files
├── src/                   # Source code for model and data processing
│   ├── data_processing.py # Scripts for data preprocessing and augmentation
│   ├── model.py           # Implementation of ResNet-D architecture
│   ├── train.py           # Training script with LR optimization and checkpointing
│   ├── utils.py           # Utility functions (metrics, logging, etc.)
├── results/               # Folder for storing trained models and logs
├── README.md              # Project README
└── requirements.txt       # Python dependencies
```

## Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/resnet-d-medical-classification.git
   cd resnet-d-medical-classification
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Prepare dataset**: Download the COVID-19 Radiography Dataset and place it in the `data/` directory.

## Training the Model

To train the ResNet-D model, use the following command:
```bash
python src/train.py --epochs 20 --batch_size 32
```

## Results

- **Accuracy**: The model achieved high accuracy across different dataset splits, with the 80/20 split yielding the best results.
- **Augmentation**: Data augmentation improved performance up to a point, with optimal results observed at 20% augmentation.

## Conclusion

This project demonstrates the potential of ResNet-D in medical image classification, achieving accurate and robust performance on lung disease detection tasks. The optimized architecture, combined with advanced training techniques, highlights how deep learning can contribute to reliable diagnostic tools in healthcare.

## References
For a complete list of references, please refer to our report.
