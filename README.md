# Crop-recommendation-system
##  Overview
This project is a **machine learning-based Crop Recommendation System** that helps farmers and agricultural experts identify the most suitable crop to grow based on environmental and soil conditions such as nitrogen, phosphorus, potassium, temperature, humidity, pH, and rainfall.

## Objectives
1. Predict the most suitable crop for given soil and climate conditions.  
2. Assist farmers in improving productivity using data-driven recommendations.  
3. Provide an interactive Streamlit web app for real-time prediction.  

##  Key Steps
1. **Data Loading & Exploration (EDA):**
   - Analyzed the distribution of crops and feature correlations.
   - Checked for missing values and outliers.

2. **Data Preprocessing:**
   - Scaled numerical features using `StandardScaler`.
   - Encoded target crop labels using `LabelEncoder`.

3. **Model Training:**
   - Used algorithms like **Random Forest** 
   - Evaluated performance using accuracy, confusion matrix, and classification report.

4. **Model Tuning:**
   - Applied `GridSearchCV` to find optimal hyperparameters.
   - Saved the best-performing model as `crop_model.pkl`.

5. **Deployment:**
   - Built an interactive web app using **Streamlit**.
   - Deployed via **ngrok** for public access through Google Colab.

---

##  Results
- Achieved high accuracy on the test dataset.  
- The model effectively recommends crops like rice, maize, cotton, etc.  
- ROC curves and confusion matrices confirm robust classification performance.


## Technologies Used
- **Python**  
- **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**  
- **Scikit-learn**, **XGBoost**  
- **Streamlit**, **ngrok** for deployment  



## How to Run (in Google Colab)
1. **Upload  trained model files**:  
   - `crop_model.pkl`  
   - `scaler.pkl`  
   - `label_encoder.pkl`

2. **Install dependencies**
   ```bash
   !pip install streamlit pyngrok joblib


