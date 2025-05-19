# AI-project-Diabetes-prediction-model
🧠 AI Diabetes Prediction Model
This repository contains a machine learning model for predicting diabetes using medical data from over 130 US hospitals collected between 1999 and 2008. The project applies various classification techniques, with the LightGBM (LGBM) classifier showing the highest accuracy.

📊 Dataset
Source: UCI Diabetes 130-US hospitals dataset

Records: 100,000+

Features: Patient demographics, diagnoses, medications, and lab results

🛠️ Features
Data preprocessing (cleaning, encoding, feature selection)

Model training and evaluation (Random Forest, LightGBM, etc.)

Performance metrics: Accuracy, Precision, Recall, F1-Score

Interactive prediction interface (optional)

No SMOTE or synthetic oversampling applied

Focuses on binary classification: Diabetic vs Non-Diabetic

🧪 Model Comparison
Model	Accuracy
Random Forest	~85%
LightGBM (LGBM)	~88%
SVM	~80%
Logistic Reg.	~78%

🚀 How to Run
1. Clone the repository
bash
Copy
Edit
git clone https://github.com/yourusername/diabetes-prediction-ai.git
cd diabetes-prediction-ai
2. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
3. Run training
bash
Copy
Edit
python train_model.py
4. Predict on new data
bash
Copy
Edit
python predict.py --input sample_patient.json
5. (Optional) Run the UI
bash
Copy
Edit
streamlit run app.py
📁 Project Structure
bash
Copy
Edit
├── data/               # Raw and cleaned datasets
├── models/             # Saved model files
├── notebooks/          # Jupyter notebooks for EDA and modeling
├── src/                # Scripts (preprocessing, training, evaluation)
├── app.py              # Streamlit app for predictions
├── train_model.py      # Script to train and save the model
├── predict.py          # Script to load model and predict
├── requirements.txt    # Python dependencies
└── README.md           # Project overview
🧠 Model Input
Example input format (JSON):

json
Copy
Edit
{
  "age": 50,
  "gender": "Male",
  "admission_type": "Emergency",
  "diagnosis": "Diabetes",
  "number_inpatient": 2,
  ...
}
📌 Goals
Improve early detection of diabetes using machine learning

Provide an easy-to-use, interactive prediction tool

Ensure high precision without synthetic data oversampling

🙌 Acknowledgements
UCI Machine Learning Repository

Scikit-learn, LightGBM, Pandas, Streamlit

Project supervised by [Your Institution or Mentor Name]

📜 License
This project is licensed under the MIT License.

Would you like to include a badge (e.g. accuracy, last updated, etc.) or a GIF screenshot of the app if you have a UI? Let me know and I can help you add that!
