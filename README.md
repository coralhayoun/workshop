# SETI Signal Classification 👽🔭
This project was part of my Bachelor's degree in Computer Science, focused on building a machine learning pipeline to classify signals from space using the [SETI (Search for Extraterrestrial Intelligence) dataset](https://www.kaggle.com/datasets/tentotheminus9/seti-data) from Kaggle.


## 🚀 Overview

The Search for Extra-Terrestrial Intelligence (SETI) is a scientific effort to detect signals from intelligent life beyond Earth. In recent years, SETI has released large volumes of radio telescope data to the public, inviting researchers and citizen scientists to explore it using modern machine learning techniques.

This project takes that mission forward by transforming radio signals into spectrogram images and framing the classification problem as an image recognition task. Using both classic and deep learning approaches, we trained models to distinguish real candidate signals from background noise — achieving a final accuracy of **92%** with a fine-tuned VGG16 neural network.


## 🧠 Technologies Used

- Python 3.x  
- NumPy & Pandas  
- Matplotlib & Seaborn  
- TensorFlow
- Scikit-learn  
- SHAP (SHapley Additive exPlanations)

## 🧪 Results

| Model| Accuracy % | Precision % (avg) | Recall % (avg) | F1-score % (avg) | Training Time (sec) | # of epoch/20 | # of Total params (+MB)
|---|---|---|---|---|---|---|---|
| logistic_regression_model | 57% | 57% | 57% | 56% | 0.289 | - | - 
| decision_tree_model | 56% | 57% | 56% | 55% | 0.0629 | - | -
| random_forest_model | 65% | 66% | 65% | 64% | 1.1899 | - | -
| resnet50_model | 14% | 2% | 14% | 4% | 418.87967467308044 | 6/20 | 27,806,599 (106.07 MB)
| resnet50_model_with_data_aug | 16% | 7% | 16% | 6% | 514.6092298030853 | 6/20 | 27,806,599 (106.07 MB)  
| vgg16_model | 62% | 76% | 62% | 59% | 747.9675004482269 | 12/20 | 15,787,847 (60.23 MB)
| vgg16_model_with_data_aug | 80% | 82% | 80% | 80% | 1584.921834230423 | 20/20 | 15,787,847 (60.23 MB)
| vgg16_model_with_data_aug_original_size | 92% | 93% | 92% | 92% | 2748.6929054260254 | 20/20 | 15,787,847 (60.23 MB)

## 📦 Installation & Exploration

This project contains large Jupyter notebook that may not render properly on platforms like [nbviewer](https://nbviewer.org) or GitHub’s native notebook viewer.

To view and interact with the notebooks properly, it’s recommended to:

1. Clone the repository
2. Open in Visual Studio Code with the [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) installed

This will allow you to:
* View the entire notebook with proper rendering
* Run cells interactively
* Explore visualizations and model outputs