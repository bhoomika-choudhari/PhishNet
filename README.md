phishnet
🛡️ PhishNet – Phishing Website Detection using ML & Deep Learning PhishNet is a powerful web-based phishing detection system that uses Artificial Neural Networks, Random Forests, and SVM to classify websites as legitimate ✅ or phishing 🚨 based on 30 key features. The system is fully deployed via a Streamlit web app with live prediction, batch processing, and visualizations.

📌 Table of Contents 🔍 Problem Statement 🚀 Proposed Work 🧠 Models Used 📊 Features & Enhancements 🗂️ Dataset 🔬 Evaluation Metrics 💻 How to Run 🌐 Deployment 📸 Screenshots

🔍 Problem Statement Phishing prediction is the task of identifying and predicting the likelihood of a website, email, or message being a phishing attempt. Several challenges arise in building a phishing detection system: #Diversity of Attacks – Evolving, social engineering, brand mimicry. #Imbalanced Data – Far fewer phishing samples than legitimate ones. #Lack of Ground Truth – Phishing sites are taken down quickly. #Limited Access to Data – Proprietary or sensitive in nature. #Feature Engineering – Selecting generalizable and robust features.

🚀 Proposed Work This project addresses the above challenges through a streamlined deep learning-based solution with multiple model comparisons.

✅ Project Workflow: -Dataset Acquisition: Downloaded phishing dataset from Kaggle. -Preprocessing: Cleaned data, handled missing values, label encoding, dropped unnecessary columns (e.g., Index, class for training). -Train-Test Split: 80% training / 20% testing. -Feature Reduction: Used PCA for dimensionality reduction. -Model Training: Trained ANN, Random Forest, and SVM classifiers. -Evaluation: Compared metrics – Accuracy, Precision, Recall, F1-Score, ROC-AUC. -Frontend: Built a full Streamlit UI for real-time interaction and insights.

🧠 Models Used: 🤖 Artificial Neural Network (ANN) – Deep learning-based classifier 🌲 Random Forest (RF) – Ensemble learning technique 📈 Support Vector Machine (SVM) – Kernel-based linear classifier

Feature	Description
✅ Real-Time Prediction	Enter 30 feature values to get instant prediction
📂 CSV Upload	Upload a CSV file and get batch predictions
📉 PCA-based Preprocessing	Feature reduction using Principal Component Analysis
📈 Evaluation Metrics	Accuracy, Precision, Recall, F1-Score, AUC
📊 ROC Curves	Interactive ROC visualization for selected model
📊 Confusion Matrix	View normalized matrix for all classifiers
📊 Comparison Chart	Bar chart comparing ANN, RF, and SVM on test data
🌙 Dark Mode (Planned)	Theme toggle support
🔎 Live URL Analyzer (Planned)	Analyze real URLs using parsing techniques
🔐 Authentication (Planned)	Secure user access to the app
🗂️ Dataset -📁 Source: Kaggle Phishing Website Dataset -🔢 Features: 30 numerical features -🎯 Target: class (0 = Legitimate, 1 = Phishing)

🔬 Evaluation Metrics All models were evaluated using the test set (20% split) and compared on the following metrics:

Metric	Description
Accuracy	Overall correctness
Precision	Correct phishing predictions out of all predicted phishing
Recall	Correct phishing predictions out of all actual phishing
F1-Score	Harmonic mean of precision and recall
ROC-AUC	Area under the ROC curve
The results are visualized in both table and bar chart formats.

💻 How to Run

Clone the repository bash Copy code '''git clone https://github.com/your-username/phishnet.git''' '''cd phishnet'''
Install dependencies bash Copy code '''pip install -r requirements.txt'''
Run the Streamlit App bash Copy code '''streamlit run frontend.py'''
🌐 Deployment You can deploy this Streamlit app on: ✅ Streamlit Cloud – Free and easy deployment 🔁 HuggingFace Spaces – Use Gradio/Streamlit ☁️ AWS/GCP/Heroku – For production-level hosting

Basic Steps for Streamlit Cloud: -Push your project to GitHub -Go to Streamlit Cloud -Click “New App” > Select repo > Choose frontend.py -Click Deploy
