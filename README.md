# Pneumonia Detection using Convolutional Neural Networks (CNN)

## Project Overview
This project aims to build a Convolutional Neural Network (CNN) model that can differentiate between normal lung images and those affected by pneumonia. The model leverages a dataset of lung X-ray images to detect health conditions, focusing on binary classification (normal vs. pneumonia). The ultimate goal is to assist in the early detection of pneumonia with high accuracy. The best model achieved an accuracy of **89%**.
 
## Dataset
The dataset used in this project consists of chest X-ray images, divided into two categories:
- **Normal lungs**
- **Lungs affected by pneumonia**

The images are resized to a resolution of **64x264** to balance performance and computational efficiency.

## Data Preprocessing
To prepare the dataset for training, the following steps were performed:

1. **Image Loading and Resizing:**
   - Images were loaded using the `load_img` function and resized to 64x264 resolution to reduce memory usage.

2. **Data Augmentation:**
   - Rotation: Randomly rotates images to improve model generalization.
   - Flipping: Horizontally flips images to increase dataset variability.
   - Zooming: Applies zoom effects to simulate different perspectives.
   - Brightness Adjustment: Varies brightness levels to account for different X-ray imaging conditions.

## Model Architecture
The CNN model includes the following layers:
1. Convolutional layers with ReLU activation functions to extract features.
2. Max-pooling layers to reduce spatial dimensions.
3. Dropout layers to prevent overfitting.
4. Fully connected layers for classification.

### Model Training
- **Loss Function:** Binary Crossentropy
- **Optimizer:** Adam
- **Evaluation Metric:** Accuracy
- **Training/Validation Split:** 80% training, 10% validation, 10% testing

## Performance
The best model achieved the following results:
- **Accuracy:** 89%
- **Loss:** Minimal validation loss with effective generalization to unseen data.

## Usage
To use this project:
1. Clone the repository:
   ```bash
   git clone https://github.com/rendra7/Computer-Vision_Pneumonia_Detection_using_CNN
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook to train the model or use the pre-trained model for inference.

## Acknowledgements
This project was inspired by the need to improve pneumonia detection and leverage deep learning techniques for medical imaging. Special thanks to the dataset providers and the open-source community for tools and libraries used in this project.

---

Feel free to contribute to this project by submitting pull requests or reporting issues. Together, we can make early detection of pneumonia more accessible and accurate!

