# Face Gender Classification Project

This project implements a face gender classification system using Transfer Learning with MobileNetV2 architecture. The model is designed to classify facial images into binary gender categories.

## Project Overview

This project utilizes deep learning techniques to perform gender classification on facial images. It leverages the MobileNetV2 architecture pre-trained on ImageNet and implements transfer learning for optimal performance.

## Technologies Used

- Python
- TensorFlow/Keras
- MobileNetV2 (Pre-trained model)
- Pandas
- NumPy
- Matplotlib

## Model Architecture

The model architecture consists of:
1. Base Model: MobileNetV2 (pre-trained on ImageNet)
2. Custom Classification Head:
   - Global Average Pooling
   - Dropout Layer (0.5)
   - Binary Classification Output

### Key Features

- Transfer Learning implementation using MobileNetV2
- Fine-tuning of the last 30 layers
- Data augmentation using ImageDataGenerator
- Validation split of 20%
- Batch processing with size of 32
- Image preprocessing to 224x224 pixels

## Data Processing

The project includes:
- Image rescaling (1/255)
- Validation split (20%)
- Batch processing
- Dynamic image loading using data generators

## Model Training Configuration

```python
Image Size: (224, 224)
Batch Size: 32
Base Model: MobileNetV2
Training Strategy: Fine-tuning last 30 layers
```

## Dataset Structure

The project expects the following data organization:
```
/content/
├── images/
│   └── [image files]
├── train.csv
├── test.csv
└── sample_submission.csv
```

## Setup and Installation

1. Clone the repository
2. Install required dependencies
3. Prepare your dataset in the required format
4. Run the training script

## Requirements

- TensorFlow
- Keras
- Pandas
- NumPy
- Matplotlib

## Usage

1. Prepare your image dataset
2. Update the data paths in the script
3. Run the training script
4. Use the trained model for predictions

## Future Improvements

- Implement additional data augmentation techniques
- Add cross-validation
- Experiment with different architectures
- Add model evaluation metrics visualization

## Author

**Depak Singh Manola** ([@manola1109](https://github.com/manola1109))

Created: 2025-05-29 20:17:08 UTC

## License

MIT License

Copyright (c) 2025 Depak Singh Manola

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Acknowledgments

- MobileNetV2 architecture from TensorFlow/Keras
- ImageNet for pre-trained weights
