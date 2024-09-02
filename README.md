# Charity Application Success Prediction Model (Neural Networks)

## Overview

This project develops a deep learning model to predict the success of funding applications for Alphabet Soup, a fictitious charity. Using TensorFlow, we build and evaluate a neural network to classify application success based on various features.

## Data Analysis

### Target Variable
- `IS_SUCCESSFUL`: Indicates whether a charity's application was successful (1) or not (0)

### Feature Variables
- `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, `ASK_AMT`

### Removed Variables
- `EIN` and `NAME`: Non-beneficial ID columns

## Model Architecture

1. **Input Layer**: Based on number of features
2. **Hidden Layers**:
   - First: 100 neurons, tanh activation
   - Second: 64 neurons, tanh activation
   - Third: 32 neurons, sigmoid activation
3. **Output Layer**: 1 neuron, tanh activation

## Model Compilation and Training

- **Optimizer**: Adam
- **Loss Function**: Binary Crossentropy
- **Epochs**: 100
- **Batch Size**: 50
- **Validation Split**: 15%

## Results

- **Accuracy**: ~70.76%
- **Loss**: ~0.0932

The model shows moderate performance in predicting application success. While achieving ~70.76% accuracy, there's room for improvement.

## Key Findings

1. The model's performance is satisfactory but not optimal.
2. The chosen architecture balances complexity and efficiency.
3. There's potential for further optimization and improvement.

## Future Work

- Experiment with different architectures and hyperparameters
- Explore alternative models or ensemble methods
- Enhance data preprocessing techniques
- Implement more advanced visualization techniques

## Quick Start

1. Install required packages: `pandas`, `sklearn`, `tensorflow`
2. Run the preprocessing script
3. Execute the model training and evaluation

For detailed implementation and full analysis, refer to the source code and accompanying documentation.
