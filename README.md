# DNN-Regression-Classification-PyTorch
This repository explores deep learning with PyTorch for regression and classification tasks. Using NYSE and predictive maintenance datasets, we perform data analysis, build neural networks, tune hyperparameters, and apply regularization techniques to optimize model performance.

# Repository Name:
DNN-Regression-Classification-PyTorch

# README Outline:
1. Project Overview
  Purpose: This project focuses on exploring and implementing deep learning techniques for regression and classification tasks using PyTorch.
  Objectives: Using exploratory data analysis, building deep neural networks, tuning hyperparameters, and applying regularization techniques for model improvement.
2. Datasets
  Part 1 - Regression: New York Stock Exchange Dataset
  Part 2 - Multi-Class Classification: Predictive Maintenance Dataset
3. Project Workflow
**  Part 1: Regression **
    1. Exploratory Data Analysis: Initial analysis and visualizations for understanding features, distribution, and relationships within the NYSE dataset.

    2. Model Building: Design of a Deep Neural Network (DNN) using PyTorch for regression.

    3. Hyperparameter Tuning: Utilization of GridSearchCV from sklearn to find optimal learning rates, optimizers, number of epochs, etc.

    4. Training & Evaluation: Training the model, and plotting Loss vs. Epochs and Accuracy vs. Epochs graphs with interpretation.

    5. Regularization Techniques: Comparison of model performance with and without regularization techniques such as Dropout, L2 Regularization, etc.

**  Part 2: Multi-Class Classification **
    1. Data Preprocessing: Cleaning, standardizing, and normalizing the Predictive Maintenance dataset.

    2. Exploratory Data Analysis: Further analysis to understand the dataset, feature relationships, and label distribution.

    3. Data Augmentation: Balancing classes through augmentation techniques.

    4. Model Building: Building a multi-class classification DNN using PyTorch.

    5. Hyperparameter Tuning: Optimizing hyperparameters for performance enhancement.

    6. Training & Evaluation: Training the model and plotting Loss vs. Epochs and Accuracy vs. Epochs graphs with interpretation.

    The training and evaluation suggest a well-trained model with high accuracy and stability, based on the plotted loss and accuracy metrics over 20 epochs. 
    
    The model demonstrated strong performance and generalization, achieving a high training accuracy of 99.16% and a stable test accuracy of 99.04% after just a few epochs. Both the            training   and test losses converged rapidly around 0.3227 and remained steady, suggesting that the model reached an optimal state early in the training process with no signs of            overfitting or        underfitting. The early plateau in accuracy and minimal gap between training and test metrics indicate that the model is well-suited for deployment, with little       to gain from additional     training. Overall, the model is efficient, accurate, and reliable for practical use.

    <img width="905" alt="Screenshot 2024-11-13 at 00 02 05" src="https://github.com/user-attachments/assets/8fa191d9-6a55-4bdf-be5f-b98e7b214fdb">


    7. Metrics Calculation: Calculation of accuracy, sensitivity, F1-score, and other metrics.

    The regularized model outperforms the original model by achieving similar high accuracy (around 99.2%) and F1 scores (0.99) on both training and test sets, but with better stability        and    generalization across epochs. The training and test losses in the regularized model are lower and converge more consistently, indicating more effective learning and reduced          overfitting.    This is evident in the close alignment between training and test metrics, which suggests that the regularization techniques improved the model’s robustness, making it a     more reliable       choice for deployment compared to the original model.

    <img width="905" alt="Screenshot 2024-11-13 at 00 23 23" src="https://github.com/user-attachments/assets/e6b74af2-debd-4f30-a9d6-4ab8ee6d530d">
