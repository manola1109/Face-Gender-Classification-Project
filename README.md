# Project Overview
Implement a binary classification model to determine gender (Male/Female) from facial images using deep learning techniques.

## Dataset Details

### Training Dataset
- Number of Images: 12,196 (70% of total data)
- Image Dimensions: 224 x 224 x 3 (RGB)

### Test Dataset
- Number of Images: 5,227 (30% of total data)
- Image Dimensions: 224 x 224 x 3 (RGB)

## Implementation Requirements

The project requires experimenting with various model architectures and hyperparameters:

### Model Architecture Variations
1. **Fully Connected (FC) Layers**
   - Experiment with different numbers of hidden layers
   - Vary the number of neurons in hidden layers

2. **Optimization Parameters**
   - Test different optimizers available in Keras
   - Experiment with various loss functions

3. **Model Configuration**
   - Try different activation functions
   - Adjust the number of training epochs

## Experimentation Matrix

Create experiments varying the following parameters:
1. Hidden Layers: [2, 3, 4] layers
2. Neurons per layer: [128, 256, 512]
3. Optimizers:
   - Adam
   - RMSprop
   - SGD
4. Loss Functions:
   - Binary Crossentropy
   - Hinge Loss
5. Activation Functions:
   - ReLU
   - LeakyReLU
   - ELU

## Expected Deliverables

1. Implemented model with the best performing configuration
2. Comparative analysis of different model configurations
3. Performance metrics on test dataset
4. Training and validation curves
5. Confusion matrix for the best model

## Success Metrics
- Model accuracy on test dataset
- F1-score
- ROC-AUC curve
- Confusion matrix analysis
