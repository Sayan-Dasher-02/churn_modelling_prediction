Customer Churn Prediction Web App

This project is a Streamlit-based web application that predicts whether a customer is likely to churn (i.e., stop using a service) based on demographic and account data.
It uses a trained Deep Learning model built with TensorFlow/Keras and preprocessing with Scikit-learn.

🚀 Features

Interactive Streamlit UI for user input.

Real-time churn probability prediction.

Uses pre-trained model and encoders for inference.

Easy to deploy locally or on cloud platforms (e.g., Streamlit Cloud, Heroku).

📁 Project Structure
Customer-Churn-Prediction/
│
├── app.py                         # Streamlit app code
├── experiment.ipynb               # Notebook for model training & experiments
├── Churn_Modelling.csv            # Dataset used for training
├── model.h5                       # Trained TensorFlow model
├── scaler.pkl                     # Scaler used for numerical features
├── label_encoder_gender.pkl       # Label encoder for Gender
├── onehot_encoder_geo.pkl         # OneHot encoder for Geography
└── README.md                      # This file
🧠 Model Overview

Framework: TensorFlow / Keras

Preprocessing: StandardScaler, LabelEncoder, OneHotEncoder

Target: Exited (1 = churn, 0 = not churn)

Inputs: CreditScore, Geography, Gender, Age, Tenure, Balance, NumOfProducts, HasCrCard, IsActiveMember, EstimatedSalary.

🧩 Requirements

Install dependencies with:

pip install -r requirements.txt

Or manually install the main packages:

pip install streamlit tensorflow scikit-learn pandas numpy

⚙️ Setup Instructions

Clone or Download this repository:

git clone https://github.com/your-username/Customer-Churn-Prediction.git
cd Customer-Churn-Prediction

Ensure the following files are present in the same directory:

model.h5
scaler.pkl
label_encoder_gender.pkl
onehot_encoder_geo.pkl

Run the Streamlit app:

streamlit run app.py

The app will open automatically in your browser.
If not, open the provided local URL (e.g., http://localhost:8501).

🧪 How to Use

Select Geography and Gender.

Adjust other input sliders or number fields.

Click Predict.

View the Churn Probability and model output message.

🧰 Troubleshooting

If you get an error about missing files, ensure your encoder .pkl and model.h5 are in the same folder as app.py.

To retrain the model, open and run experiment.ipynb.

If the encoders show mismatch errors, re-fit and re-save them using the same preprocessing logic.

📜 License

This project is released under the MIT License.
Feel free to use, modify, and distribute with attribution.
