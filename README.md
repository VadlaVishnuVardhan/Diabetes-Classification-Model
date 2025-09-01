# Diabetes Prediction 

This project predicts whether a person has diabetes or not using machine learning models. The dataset used is publicly available on Kaggle.  

##  Dataset  
- Source: [Kaggle - Diabetes Dataset](https://www.kaggle.com/johndasilva/diabetes)  
- Features include:
  - Pregnancies  
  - Glucose  
  - Blood Pressure  
  - Skin Thickness  
  - Insulin  
  - BMI  
  - Diabetes Pedigree Function (DPF)  
  - Age  

## ⚙ Project Workflow  
1. **Exploratory Data Analysis (EDA)**  
   - Visualized distributions and relationships among features.  
   - Checked correlations and missing values.  

2. **Data Cleaning**  
   - Handled missing/invalid entries.  
   - Normalized and scaled feature values.  

3. **Model Building**  
   - Tried multiple classifiers: Logistic Regression, Decision Tree, Random Forest, etc.  
   - Evaluated performance using accuracy, confusion matrix, and classification report.  
   - Selected **Random Forest** as the best-performing model.  

4. **Hyperparameter Tuning**  
   - Fine-tuned Random Forest parameters to improve accuracy.  

5. **Prediction Function**  
   - Created a `predict_diabetes()` function to classify new patient data.  
   - Example inputs:
     ```python
     prediction = predict_diabetes(2, 81, 72, 15, 76, 30.1, 0.547, 25)
     if prediction:
         print("Oops! You have diabetes.")
     else:
         print("Great! You don't have diabetes.")
     ```

##  Results  
- **Random Forest** achieved the highest accuracy among all tested models.  
- Provides quick predictions for unseen data.  
