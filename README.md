# ResNet-D for medical image classification

## Project Overview
Medical image classification plays a crucial role in healthcare by helping in early disease detection and diagnosis. This project uses ResNet-D to classify lung conditions based on X-ray scans. Our study focuses on optimizing the ResNet-D model to accurately classify medical images, highlighting enhancements in feature extraction and model accuracy through advanced training techniques and data augmentation.

## Team members
- Nguyen Quang Huy
- Nguyen Tuan Khai
- Nguyen Hai Dang
- Pham Thai Son

## Dataset
The model uses the [COVID-19 Radiography Dataset](https://www.kaggle.com/datasets/preetviradiya/covid19-radiography-dataset), which includes X-ray images for:
- COVID-19 positive cases
- Normal cases
- Viral Pneumonia cases
- Lung Opacity cases

## Image Processing
- Resize the image into 224 x 224
- Convert the input images to PyTorch tensors, which are multi-dimensional arrays representing the image data.
- Normalize the image tensor to a predefined mean and standard deviation across each channel.

## Results
The model achieved high accuracy across different dataset splits, with the 80/20 split yielding the best results.<br>By using model improvements like advanced learning rate and data augmentation, the model shows a significant improvement with 20% data augmented.

## References
Please refer to our report for a complete list of references.

