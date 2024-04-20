# Image Classification with TensorFlow

## Overview
This repository contains a Python script for image classification using TensorFlow. The script is designed to classify images into two categories: "batagor" and "bukan".

## Requirements
- Python 3.x
- TensorFlow
- Matplotlib
- NumPy
- PIL
- scikit-learn

## Usage
1. Clone this repository to your local machine:

    ```
    git clone https://github.com/your_username/your_repository.git
    ```

2. Navigate to the cloned directory:

    ```
    cd your_repository
    ```

3. Run the Python script `image_classification.py`:

    ```
    python image_classification.py
    ```

4. The script will display sample images from the training dataset and then train the image classification model. Once training is complete, it will evaluate the model's performance using the validation dataset and display the classification report.

## Dataset
The dataset used in this project consists of images of "batagor" and "bukan" categories. The images are divided into training and validation sets, stored in separate directories:

- Training images:
  - `train/batagor`: Contains images of batagor
  - `train/bukan`: Contains images of bukan
- Validation images:
  - `validation/batagor`: Contains images of batagor
  - `validation/bukan`: Contains images of bukan

## Model Architecture
The image classification model is built using TensorFlow and consists of the following layers:
- Input layer: Accepts images with dimensions (150, 150, 3)
- Flatten layer: Flattens the input image
- Dense layer: Fully connected layer with 512 units and ReLU activation
- Output layer: Fully connected layer with 2 units and sigmoid activation (for binary classification)

## Training
The model is trained using the training dataset with the following configurations:
- Batch size: 32
- Epochs: 55
- Optimizer: RMSprop (learning rate = 0.001)
- Loss function: Binary cross-entropy
- Metrics: Accuracy

## Evaluation
The trained model is evaluated using the validation dataset, and the following metrics are calculated:
- Accuracy
- Classification report: Provides precision, recall, F1-score, and support for each class

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to customize this README file further based on your specific project details and requirements! Let me know if you need any further assistance!
