# 🖼️ CIFAR-10: Deep Learning Image Classification with CNN

## 🔍 Introduction
This project is part of Group 5's work on developing advanced image classification models using the CIFAR-10 dataset. We explored two primary approaches: building a custom Convolutional Neural Network (CNN) and implementing transfer learning with the pre-trained DenseNet-121 model.

## 👥 Team Members
- **Diego Inclan**
- **Saiqa Mehdi**
- **Katharina Krux**

## 📂 Project Structure

```plaintext
/
├── models/             # Serialized models and training configurations
├── notebooks/          # Development Jupyter notebooks
├── src/                # Source code for model training and data preprocessing
├── images/             # Images used for documentation
├── reports/            # Complete project reports and additional documentation
└── README.md           # Project overview and setup instructions
```


## 📝 Project Description

We tackled the CIFAR-10 dataset, which comprises 60,000 32x32 color images across 10 classes. Our goal was to compare the effectiveness of a custom CNN against a sophisticated pre-trained network, focusing on overcoming challenges like data quality and model overfitting.

## 🔄 Data Preprocessing
- **Grayscale Conversion**: Applied to the custom model to reduce complexity.
- **Normalization**: Pixel values scaled to [0, 1] range.
- **Data Augmentation**: Included rotations and flips to minimize overfitting.
- **Resizing**: Necessary for adapting CIFAR-10 images to the DenseNet input requirements.

## 🤖 Models

### 1. Custom CNN:

- **Architecture**: Sequential layers including convolutional blocks, batch normalization, pooling, and fully connected layers.
- **Training**: Utilized the Adam optimizer with a learning rate of 0.001, and categorical crossentropy as the loss function.

### 2. Transfer Learning with DenseNet-121:

- **Modifications**: Adapted DenseNet-121 to handle the smaller image size of CIFAR-10 by resizing images and adjusting the top layers.
- **Augmentation**: Enhanced with random zoom and contrast adjustments for robustness.

## 📈 Training and Evaluation

- **Early Stopping**: Used to halt training when validation loss ceased to decrease, preventing overfitting.
- **Metrics**: Tracked accuracy, precision, recall, and F1-score across training and validation phases.
  
## 📊 Results
Our models demonstrated substantial learning capabilities, though they encountered limits in validation accuracy due to inherent dataset challenges. Insights into class-specific performance were gained through confusion matrices, revealing frequent misclassifications among similar categories.

## 💡 Insights and Future Directions
- **Importance of Preprocessing**: Effective preprocessing significantly influences model performance.
- **Hyperparameter Tuning**: Systematic tuning was crucial for optimizing model outcomes.
- **Transfer Learning Efficiency**: DenseNet-121 showed promise but required careful tuning to adapt to CIFAR-10.

## 🎯 Conclusion

Both models provided valuable learning experiences in handling image data and model optimization. Continued exploration could include more aggressive hyperparameter tuning or trials with other advanced architectures like Vision Transformers.

## 🛠️ How to Use

To replicate our findings or use the models:
1. Clone the repository.
2. Install dependencies listed in requirements.txt.
3. Run the Jupyter notebooks within the notebooks/ directory.

## 📄 Report
For a detailed breakdown of the project's phases, results, and methodologies, please refer to the comprehensive report available in the reports/ directory.

## ©️ License
This project is licensed under the MIT License. See the LICENSE.md file for details.








