# Transfer Learning for Cotton Plant Disease Detection

## Project Overview
This project applies transfer learning techniques to tackle the problem of detecting diseases in cotton plants using image data. The goal is to leverage pre-trained models to identify and classify fresh and diseased cotton plants and leaves, contributing to efforts in combating climate-related challenges in agriculture.

## Dataset Description
The dataset includes images categorized into four classes:
- Fresh Cotton Plant
- Fresh Cotton Leaf
- Diseased Cotton Plant
- Diseased Cotton Leaf

These images are split into training, validation, and testing sets, facilitating the model training and evaluation process.

## Models Used
The following pre-trained models from TensorFlow's Keras Applications are fine-tuned:
- **Inception V3**: Known for its efficiency with a smaller number of parameters. It's suitable for mobile and web applications given its balance between speed and accuracy.
- **ResNet 50**: Offers a deep architecture, particularly effective for more complex image classification tasks due to its residual learning features.
- **ResNet 152 V2**: An extended version of ResNet 50 with more layers, enhancing its ability to learn from a larger set of features, ideal for highly detailed image classification.

## Implementation
Each model is fine-tuned for the specific task of classifying cotton plant images. We modify the top layers of each network to suit our four-class problem and employ techniques such as data augmentation and learning rate adjustments to enhance training outcomes.

### Notebooks
- `Transfer_Learning_Inception_V3.ipynb`
- `Transfer_Learning_Resnet_50.ipynb`
- `Transfer_Learning_Resnet152V2.ipynb`

Each notebook contains detailed steps for loading the model, performing fine-tuning, and evaluating the results.

## Evaluation Metrics
Model performance is assessed using several metrics:
- Accuracy
- Loss
- Precision
- Recall
- F1 Score

## Results and Discussion
The findings from fine-tuning different models are presented, discussing the strengths and limitations of using transfer learning for plant disease detection. A comparative analysis highlights which models perform best based on the evaluation metrics.

## Conclusion
This project demonstrates the potential of transfer learning in improving the detection of diseases in cotton plants, contributing to sustainable agricultural practices in the face of climate change challenges.
