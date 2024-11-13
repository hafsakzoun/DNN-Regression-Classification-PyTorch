# DNN-Regression-Classification-PyTorch

This repository demonstrates the application of deep learning with PyTorch for both regression and classification tasks. Using the NYSE stock data and Predictive Maintenance datasets, we explore data, build neural network models, fine-tune hyperparameters, and apply regularization techniques to improve model performance and generalization.

> **Note**: All code and outputs are available in the attached files for easy reference and replication.

---

## Repository Outline

### 1. Project Overview
   - **Purpose**: Showcase the use of deep learning techniques to solve regression and classification problems using PyTorch.
   - **Objectives**: Analyze datasets, design neural networks, optimize model performance through hyperparameter tuning, and apply regularization techniques to enhance model robustness.

### 2. Datasets
   - **Part 1 - Regression**: NYSE Stock Dataset for predicting stock prices.
   - **Part 2 - Multi-Class Classification**: Predictive Maintenance Dataset for fault prediction.

---

## Project Workflow

### Part 1: Regression (NYSE Stock Dataset)

1. **Exploratory Data Analysis**: 
   - **Data Overview**: 
      - `prices` and `pricesSplitAdjusted`: Around 850,000 rows, providing open, close, low, high prices, and volume for various stocks.
      - `securities`: Contains company information like GICS Sector and Sub Industry (505 rows).
      - `fundamentals`: Includes 1,781 rows with financial metrics like Total Revenue and Net Income.
   - **Summary Statistics**:
      - Stock prices: Average open and close prices around $70; volume varies widely.
      - Financial metrics: Variance in metrics (e.g., Accounts Payable, Total Revenue) reflects differences in company size.

   ![Data Visualization](https://github.com/user-attachments/assets/)

2. **Model Building**:
   - **Data Splitting**: Data is divided into 80% training and 20% testing sets.
   - **DNN Model Architecture**:
      - A deep neural network (DNN) with one input layer, three hidden layers (128, 64, 32 neurons), and one output layer, with ReLU activation functions for hidden layers.
   - **Training Progress**:
      - Training over 100 epochs showed a significant decrease in training loss, reaching near-zero (0.0002), indicating effective learning.
   - **Model Evaluation**:
      - The model achieved a low root mean squared error (RMSE) of 0.0142 on the test set, suggesting accurate prediction on unseen data.

3. **Hyperparameter Tuning**: 
   - Used `GridSearchCV` from `sklearn` to optimize learning rate, optimizer type, number of epochs, and architecture configurations.

4. **Training & Evaluation**:
   - Plots for **Loss vs. Epochs** and **Accuracy vs. Epochs** provide insight into model learning and convergence.

5. **Regularization Techniques**:
   - Techniques like Dropout and L2 Regularization were applied to improve model performance and prevent overfitting.

### Part 2: Multi-Class Classification (Predictive Maintenance Dataset)

1. **Data Preprocessing**: 
   - Cleaned, standardized, and normalized the dataset to prepare it for classification.

2. **Exploratory Data Analysis**:
   - Analyzed relationships between features and the distribution of target classes.

3. **Data Augmentation**:
   - Employed augmentation techniques to balance class distribution for better model learning.

4. **Model Building**:
   - Developed a multi-class classification DNN model in PyTorch.

5. **Hyperparameter Tuning**:
   - Tuned model parameters (learning rate, optimizer, etc.) to achieve optimal results.

6. **Training & Evaluation**:
   - The model achieved high stability with 99.16% accuracy on the training set and 99.04% on the test set, demonstrating early convergence and minimal overfitting.

   ![Model Accuracy Graph](https://github.com/user-attachments/assets/8fa191d9-6a55-4bdf-be5f-b98e7b214fdb)

7. **Metrics Calculation**:
   - Evaluated key metrics like accuracy, sensitivity, F1-score, and others for a comprehensive assessment.

8. **Regularized Model Performance**:
   - Applying regularization yielded improved accuracy (99.2%) and convergence stability across epochs, showing enhanced model generalization.

   ![Regularized Model Graph](https://github.com/user-attachments/assets/e6b74af2-debd-4f30-a9d6-4ab8ee6d530d)

---

For more detailed insights and results, please explore the code and outputs provided in the attached files.
